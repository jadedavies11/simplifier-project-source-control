# FHIR Messaging
<div style="float:right;border:1px;border-style:solid;padding:10px;margin:10px;width:300px;">

  - [Context of Use](#context-of-use)
  - [Data Model Overview](#data-model-overview)
  - [FHIR Resources](#fhir-resources)
    * [Bundle](#bundle)
    * [MessageDefinition](#messagedefinition)
    * [MessageHeader](#messageheader)
    * [OperationOutcome](#operationoutcome)
    * [Resource (any)](#resource-any)
  - [Resource Identification](#resource-identification)
  - [Message Events and Handling](#message-events-and-handling)
  - [FHIR Messaging Examples](#fhir-messaging-examples)
</div>

## Context of Use
The FHIR messaging paradigm facilitates the transmission of multiple related resource profiles via a single message bundle, in accordance with a message definition defined for the specific purpose of the message.  

Applications using FHIR messaging may have knowledge of existing FHIR resource instances and their logical identifiers, or they may use other stable identifiers to uniquely identify the referenced entities.

FHIR messaging is the preferred mechanism for data submissions to the all-Wales Care Data Repository (CDR). For each interacting application type, a CDR message handler will accept FHIR bundle submissions via API for specific message events. The handler will resolve references for pre-existing resource instances and will create or update resource instances as appropriate, including any associated provenance records. The outcome of the data submission will be returned together with the logical identities of the resources created, updated or resolved.

The specific content of the response messages to be used by the CDR and any associated error codes are beyond the scope of this guidance. 

## Data Model Overview
The FHIR messaging paradigm uses FHIR resources to orchestrate and validate the content of a message. There are four key resources, plus any number of involved FHIR resource types, as applicable to the purpose of the message.

The FHIR data model consists of the following resources: 
* [Bundle](https://www.hl7.org/fhir/R4/bundle.html) 
* {{pagelink:DataStandardsWales-MessageDefinition, text:MessageDefinition}}
* {{pagelink:DataStandardsWales-MessageHeader, text:MessageHeader}}
* [OperationOutcome](https://www.hl7.org/fhir/R4/operationoutcome.html) 
* Resource (any)

<br />
{{render:Diagrams-FHIR-Messaging-Data-Model}}
<br />

Note: It may be appropriate to omit the bundle entry for a resource instance where a logical ID is known and provided in the focus.

## FHIR Resources
### Bundle
In the context of FHIR messaging, a Bundle resource of type “message” is used to convey the data payload as a series of FHIR resources (entries). The first entry must be a message header as this defines the purpose of the messaging bundle instance. The remaining entries must contain valid resource profile instances.

### MessageDefinition
A MessageDefinition resource is used to constrain the message header content for a specific message event. It applies upper and lower bounds to the number of resource instances of each profile that can be referenced as a focus of the message header.

### MessageHeader
The message header of a message bundle identifies the specific involved resources, constrained by the types, profiles and cardinalities specified in the referenced message definition. It defines the source endpoint from which the bundle originated and the specific message event to be processed by the recipient. It can also carry other information relevant to the provenance of the information contained within the bundle, such as:
* one or more destinations for the message
* the sender
* the enterer
* the author
* the responsible Organization

The message header is also used to convey the response to the submission.

### OperationOutcome
An operation outcome resource is referenced from the message header to convey details of all issues encountered in processing the bundle content. The issues may be hints, warnings or errors and should include identification of the resource element that caused the issue. As specific error codes have been defined within this guide.

### Resource (any)
A FHIR messaging bundle for a message event will include all involved resources as focus elements. In the following cases the resource profile must also be included as a bundle entry:
* any resource to be created or updated
* any referenced resource for which the resource Id within the CDR is not known

## Resource Identification
A key feature of FHIR is the ability of resources to reference each other. This is done using the Reference data type. This data type supports two modes of referencing:
* Literal references, using the .reference element. In this case a relative or absolute REST endpoint containing the .id of the referenced resource is used. In a Bundle context, this may also be a reference to a Bundle.entry.fullUrl.
* Logical references, using the .identifier element. Such a reference entails a match on the business identifier (.identifier) for the referenced resource, without specifying where to find the referenced resource.

## Message Events and Handling
Each message handler will process a set of predefined message events and associated message definitions according to the business rules for the specific use case.  These rules will include protocols for handling referenced entities not currently known to the CDR, determining for example whether the referenced entity is created as a new FHIR resource instance, treated as an error or processed with a warning.
<br /><br />
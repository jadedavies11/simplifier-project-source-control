# Documents
<div style="float:right;border:1px;border-style:solid;padding:10px;margin:10px;width:300px;">

  - [Data Model Overview](#data-model-overview)
  - [FHIR Resources](#fhir-resources)
    * [Device](#device)
    * [DocumentReference](#documentreference)
    * [Encounter](#encounter)
    * [Location](#location)
    * [Organization](#organization)
    * [Patient](#patient)
    * [PractitionerRole](#practitionerrole)
    * [Provenance](#provenance)
  - [Supporting Legacy Metadata](#supporting-legacy-metadata)
  - [Clinical Scenarios / Examples](#clinical-scenarios-examples)
    * [Encounter-based Document](#encounter-based-document)
    * [Event-based Document](#event-based-document)
    * [Document not Event-based](#document-not-event-based)
    * [Examples](#examples)
  - [Document Error Workflow](#document-error-workflow)
    * [Misfiling Workflow](#misfiling-workflow)
    * [Revocation Workflow](#revocation-workflow)
</div>

## Data Model Overview
The metadata associated with patient care documents will be stored as a dedicated DocumentReference resource and, where appropriate, as a linked Encounter resource specific to the documented event. Many aspects of the metadata will be achieved through referencing of pre-existing administrative entities such as Device, Organisation and PractitionerRole. The creation or update of a DocumentReference instance will be associated with one or more Provenance resource instances, targeting the specific version of the DocumentReference instance. 

The diagram below provides an overview of the required FHIR resources and how they can be interconnected to support a range of document metadata use cases. It shows that there are multiple places in which key event metadata such as Event site and Event location may be stored, dependent upon the specific use case. See the dedicated clinical scenario guidance for recommendations on the tailoring of the data model for different circumstances. 

The FHIR data model consists of the following resources: 
* {{pagelink:DataStandardsWales-Device,text:Device}} 
* {{pagelink:DataStandardsWales-DocumentReference,text:DocumentReference}} 
* {{pagelink:DataStandardsWales-Encounter,text:Encounter}} 
* {{pagelink:DataStandardsWales-Location,text:Location}}
* {{pagelink:DataStandardsWales-Organization,text:Organization}}
* {{pagelink:DataStandardsWales-Patient,text:Patient}}
* {{pagelink:DataStandardsWales-PractitionerRole,text:PractitionerRole}}
* {{pagelink:DataStandardsWales-Provenance,text:Provenance}}
<br />
{{render:Diagrams-Document-metadata-maximal-logical-model}}
<br />

## FHIR Resources
### Device
The source system that provided the document details will be represented as a Device resource instance.

### DocumentReference
Each DocumentReference resource instance represents a distinct document. In addition to information about the document, the DocumentReference provides a URL to the location from which the document can be retrieved. For those familiar with the Welsh Care Records Service, the DocumentReference instance represents the document supersession set.

### Encounter
The documented event may be represented as an Encounter resource instance. In this case applications may access the referenced Encounter to retrieve the event details including document metadata such as event site and event organisation.

### Location
There are two roles that may be fulfilled by a location, as represented by a Location resource instance. The first is the event site, and the second a more specific event location. For example the event location may be a specific ward within a hospital identified as the event site.

### Organization
There are two roles that may be fulfilled by an organisation, as represented by an Organization resource instance. The first is the custodian organisation: the health board responsible for the document, which relates to one of their patients. The second role is as the event organisation i.e. the health board that provided care via the documented event. 

### Patient
Documents will typically have a subject that is a Patient resource instance.

### PractitionerRole
Ideally the staff involved with the document as author, attester or committer can be referenced via a PractitionerRole resource instance. This facilitates access to richer contextual data than if the Practitioner resource is directly referenced.

### Provenance
The Provenance resource provides an audit trail of when a specific document version was committed and by whom. If patient demographics are also submitted, these are captured in an additional Provenance instance that specifically captures demographics as recorded, to support retrospective analysis. See the dedicated guidance page for clarification of the purpose and use of the Provenance resource:
* {{pagelink:Home/Guidance/Provenance/Index.page.md, text: Provenance Guidance}}

## Supporting Legacy Metadata
Legacy care documents may have associated metadata that are not explicitly covered by the formal content of the DocumentReference or its related resources. In order to avoid data loss on migration, a complex extension has been included called documentAttribute. To mitigate against uncontrolled proliferation of document metadata, the attribute name code has been locked down to known attribute names from the Welsh Care Records Service that are not addressed in more formal ways.

<br />
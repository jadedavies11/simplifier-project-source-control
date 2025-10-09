# {{page-title}}

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
  - [Document Error Workflow](#document-error-workflow)
  - [Supporting Legacy Metadata](#supportimg-legacy-metadata)
</div>

## Data Model Overview
The FHIR-based Clinical Data Repository (CDR) will carry metadata for a range of documents related to the clinical care of individual patients.  The metadata will be stored as a dedicated DocumentReference resource and where appropriate as a linked Encounter resource specific to the documented event.  Many aspects of the metadata will be achieved through referencing of pre-existing administrative entities such as Device, Organisation and PractitionerRole.  The creation or update of a DocumentReference instance will be associated with one or more Provenance resource instances, targetting the specific version of the DocumentReference instance.  

The diagram below provides an overview of the required FHIR resources and how they can be interconnected to support a range of document metadata use cases.  It shows that there are multiple places in which key event metadata such as Event site and Event location may be stored, dependent upon the specific use case.  See the dedicated clinical scenario guidance for recommendations on the tailoring of the data model for different circumstances. 

The FHIR data model consists of the following resources: 
* {{pagelink:DataStandardsWales-DocumentReference,text:DocumentReference}} 
* {{pagelink:DataStandardsWales-Encounter,text:Encounter}} 
* {{pagelink:DataStandardsWales-Patient,text:Patient}}
* {{pagelink:DataStandardsWales-Organization,text:Organization}}
* {{pagelink:DataStandardsWales-Location,text:Location}}
* {{pagelink:DataStandardsWales-PractitionerRole,text:PractitionerRole}}
* {{pagelink:DataStandardsWales-Device,text:Device}} 
* {{pagelink:DataStandardsWales-Provenance,text:Provenance}}


{{render:Diagrams-Document-metadata-maximal-logical-model}}

<br />

Note that the identfied resources are those expected to be applicable for the majority of patient clinical documents.  Alternative resources can be referenced in accordance with the FHIR standard for the element supporting the metadata item:
- Subject: Patient | Practitioner | Group | Device
- Author: PractitionerRole | Practitioner | Organization | Device | Patient | RelatedPerson
- Authenticator: PractitionerRole | Practitioner | Organization | Patient
- Committer: PractitionerRole | Practitioner | Organization | Device | Patient | RelatedPerson
- Senior Responsible Clinician: PractitionerRole | Practitioner  

<br />

## FHIR Resources
The resources below are presented in a logical order, according to their role within the document metadata.

### DocumentReference
Each DocumentReference resource instance represents a distinct document.  Newer versions of the same document "overwrite" the existing version, which becomes accessible only via the version history of the DocumentReference resource instance. In addition to information about the document, the DocumentReference provides a URL to the location from which the document can be retrieved.

### Encounter
The documented event may be represented as an Encounter resource instance.  In this case applications may access the referenced Encounter to retrieve the event details including document metadata such as event site and event organisation.

### Patient
Documents will typically have a subject that is a Patient resource instance.

### Organization
There are two roles that may be fulfilled by an organisation, as represented by an Organization resource instance.  The first is the custodian organisation: the health board responsible for the document, which relates to one of their patients.  The second role is as the event organisation i.e. the health board that provided care via the documented event.  

### Location
There are two roles that may be fulfilled by a location, as represented by a Location resource instance.  The first is the event site, and the second a more specific event location.  For example the event location may be a specific ward within a hospital identified as the vent site.

### PractitionerRole
Ideally the staff involved with the document as author, attester or committer can be referenced via a PractitionerRole resource instance.  This facilitates access to richer contextual data than if the Practitioner resource is directly referenced.

### Device
The source system that provided the document details will be represented as a Device resource instance.

### Provenance
The Provenance resource provides an audit trail of when a specific document version was updated and by whom.  If patient demographics are also submitted, these are captured in an additional Provenance instance that specifically captures demographics as recorded, to support retrospective analysis.  

<br />

## Document Error Workflow
There are existing processes via which a document may cease to be valid as part of a patient's record such as the document misfile workflow supported by the Welsh Clinical Portal and explicit document revocation.  Such documents usually need to remain visible with their error status clearly marked.  There will typically be restrictions on the further use of these invalid documents.

In all cases, the mandatory DocumentReference.status element for such a document should be set to "entered-in-error".  An additional errorStatus has been added as an extension and should be set to the appropriate value accrding to the error action performed.  An additional extension for errorAction offers the opportunity to record which error action type was performed, when, by whom and for what reason.

For coherence, it is recommended that the error status and status be set according to the last error action performed as in the table below:

| Last error action (actionType) | errorStatus           | status                 |
| :--- | :------ | :------ |
| revoked | revoked | entered-in-error |
| misfile-proposed | potential-misfile | entered-in-error |
| misfile-accepted | misfiled | entered-in-error |
| misfile-rejected |  | current |

It is also recommended that DocumentReference.docStatus is not changed.  This is to preserve the composition status value in case the document is subsequently reinstated.

Click {{pagelink:Example-DataStandardsWales-DocumentReference-MisfiledNotEventBased, text: here}} for an example of the population of status and error-related elements in a DocumentReference for a document that has been misfiled.  For clarity, this example represents subsequent misfiling of a final document that is not event-based, as per the example {{pagelink:Example-DataStandardsWales-DocumentReference-NotEventBased, text: here}}.  

<br />

## Supporting Legacy Metadata
Legacy documents may have associated metadata that are not explicitly covered by the formal content of the DocumentReference or its related resources.  In order to avoid data loss on migration, a complex extension has been included called documentAttribute.  This will flexibly accommodate an attribute name code, a value, a value domain and a namespace.  To avoid uncontrolled proliferation of document metadate, the attribute name code has been locked down to known attribute names from the Welsh Care Records Service that are not addressed in more formal ways.

<br />



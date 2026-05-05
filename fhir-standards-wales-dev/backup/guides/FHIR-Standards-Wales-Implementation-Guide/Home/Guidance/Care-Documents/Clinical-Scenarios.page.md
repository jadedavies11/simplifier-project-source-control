# Clinical Scenarios / Examples
## Encounter-based Document
### Overview
This scenario addresses the use of FHIR resources to fulfil the metadata requirements for a document that is based on an event represented as an Encounter resource. An example might be an outpatient clinic attendance.

### Implementation Guidance
In this case, the document metadata specific to the documented event belong to the Encounter resource, so the recommendation would be to avoid storing them within the Document Reference resource instance as this would be data duplication:
- Event Date and Time
- Event Organisation
- Event Site
- Event Location
- Event Senior Responsible Clinician

### Logical Model
The diagram below shows how the FHIR resources work together to provide the event and other metadata for a document that fits this clinical scenario.
<br />
{{render:Diagrams-Document-metadata-encounter-based}}
<br />

## Event-based Document
### Overview
This scenario addresses the use of FHIR resources to fulfil the metadata requirements for a document that is based on an event that is not represented as an Encounter resource. An example might be a historic outpatient clinic attendance.

### Implementation Guidance
In this case, the document metadata specific to the documented event must be explicit within the DocumentReference resource instance. The recommendation is to use the relevant sub-elements of the `DocumentReference.context` backbone element to capture the following event metadata:
- Event Date and Time
- Event Organisation
- Event Site
- Event Location
- Event Senior Responsible Clinician

### Logical Model
The diagram below shows how the FHIR resources work together to provide the event and other metadata for a document that fits this clinical scenario.
<br />
{{render:Diagrams-Document-metadata-event-based}}
<br />

## Document not Event-based 
### Overview
This scenario addresses the use of FHIR resources to fulfil the metadata requirements for a document that is pertinent to the clinical record but not based on a clinical event. An example might be a statement of medical insurance cover.

### Implementation Guidance
In this case, the following metadata items can be omitted: 
- Event Date and Time
- Event Organisation
- Event Site
- Event Location
- Event Senior Responsible Clinician

### Logical Model
The diagram below shows how the FHIR resources work together to provide the metadata for a document that fits this clinical scenario. The model is simplified to omit the event metadata.
<br />
{{render:Diagrams-Document-metadata-not-event-based}}
<br />

## Examples
### DocumentReference
The following examples represent DocumentReference resources for the three scenarios outlined in the preceding sections:
* {{pagelink:Example-DataStandardsWales-DocumentReference-EncounterBased, text: Example Document Reference - Encounter-based}}
* {{pagelink:Example-DataStandardsWales-DocumentReference-EventBased, text: Example Document Reference - Event-based}}
* {{pagelink:Example-DataStandardsWales-DocumentReference-NotEventBased, text: Example Document Reference - Not event-based}}

### Provenance
The following examples represent Provenance resource instances for a newly created DocumentReference for which patient demographics were provided:
* {{pagelink:Example-DataStandardsWales-Provenance-DocumentReferenceCreation, text: Example Provenance for DocumentReference creation}}
* {{pagelink:Example-DataStandardsWales-Provenance-DocumentReferenceDemographics, text: Example Provenance for demographics as recorded with care document}}

<br />
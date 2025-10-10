# Clinical Scenarios
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

{{render:Diagrams-Document-metadata-encounter-based}}

### Example Document Reference
The following example is a DocumentReference for this clinical scenario.
* {{pagelink:Example-DataStandardsWales-DocumentReference-EncounterBased, text: Example Document Reference - Encounter-based}}

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

{{render:Diagrams-Document-metadata-event-based}}

### Example Document Reference
The following example is a DocumentReference for this clinical scenario.
* {{pagelink:Example-DataStandardsWales-DocumentReference-EventBased, text: Example Document Reference - Event-based}}

## Document not Event-based 
### Overview
This scenario addresses the use of FHIR resources to fulfil the metadata requirements for a document that is pertinent to the clinicial record but not based on a clinical event. An example might be a statement of medical insurance cover.

### Implementation Guidance
In this case, the document metadata specific to the documented event can be omitted: 
- Event Date and Time
- Event Organisation
- Event Site
- Event Location
- Event Senior Responsible Clinician

### Logical Model
The diagram below shows how the FHIR resources work together to provide the metadata for a document that fits this clinical scenario. The model is simplified to omit the event metadata.

{{render:Diagrams-Document-metadata-not-event-based}}

### Example Document Reference
The following example is a DocumentReference for this clinical scenario.
* {{pagelink:Example-DataStandardsWales-DocumentReference-NotEventBased, text: Example Document Reference - Not Event-based}}

<br />
# {{page-title}}

## Overview
This scenario addresses the use of FHIR resources to fulfil the metadata requirements for a document that is based on an event represented as an Encounter resource.  An example might be an outpatient clinic attendance.


## Implementation Guidance
In this case, the document metadata specific to the documented event belong to the Encounter resource, so the recommendation would be to avoid storing them within the Document Reference resource instance as this would be data duplication:
- Event Date and Time
- Event Organisation
- Event Site
- Event Location
- Event Senior Responsible Clinician


### Logical Model
The diagram below shows how the FHIR resources work together to provide the event and other metadata for a document that fits this clinical scenario.

{{render:Diagrams-Document-metadata-encounter-based}}
<br />

### Example Document Reference
Click {{pagelink:Example-DataStandardsWales-DocumentReference-EncounterBased, text: here}} for an example of a DocumentReference that fits this clinical scenario.

<br />

# {{page-title}}

## Overview
This scenario addresses the use of FHIR resources to fulfil the metadata requirements for a document that is pertinent to the clinicial record but not based on a clinical event.  An example might be a statement of medical insurance cover.


## Implementation Guidance
In this case, the document metadata specific to the documented event can be omitted: 
- Event Date and Time
- Event Organisation
- Event Site
- Event Location
- Event Senior Responsible Clinician


### Logical Model
The diagram below shows how the FHIR resources work together to provide the metadata for a document that fits this clinical scenario. The model is simplified to omit the event metadata.

{{render:Diagrams-Document-metadata-not-event-based}}
<br />

### Example Document Reference
Click {{pagelink:Example-DataStandardsWales-DocumentReference-NotEventBased, text: here}} for an example of a DocumentReference that fits this clinical scenario.

<br />

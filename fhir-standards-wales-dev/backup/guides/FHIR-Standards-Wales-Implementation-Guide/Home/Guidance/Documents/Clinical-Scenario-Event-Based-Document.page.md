# {{page-title}}

## Overview
This scenario addresses the use of FHIR resources to fulfil the metadata requirements for a document that is based on an event that is not represented as an Encounter resource.  An example might be a historic outpatient clinic attendance.


## Implementation Guidance
In this case, the document metadata specific to the documented event must be explicit within the DocumentReference resource instance.  The recommendation is to use the relevant sub-elements of the `DocumentReference.context` backbone element to capture the following event metadata:
- Event Date and Time
- Event Organisation
- Event Site
- Event Location
- Event Senior Responsible Clinician


### Logical Model
The diagram below shows how the FHIR resources work together to provide the event and other metadata for a document that fits this clinical scenario.

{{render:Diagrams-Document-metadata-event-based}}
<br />

### Example Document Reference
Click {{pagelink:Example-DataStandardsWales-DocumentReference-EventBased, text: here}} for an example of a DocumentReference that fits this clinical scenario.

<br />

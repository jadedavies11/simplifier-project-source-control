# FHIR Messaging Examples
## Add a Professional (WCP)
### Overview
This scenario illustrates the message bundle required to submit details of a new clinician to the CDR.  The following details apply:

| Data point | Value |
| ------ | ------ | 
| name | Dr Joe Allan Bloggs |
| Professional registration | GMC:123456 |
| Nadex | Jo123456 |
| Employer organisation | Cardiff and Value University Health Board |

### Implementation Guidance
The submission of a clinician is governed by a message definition that requires exactly one of each of the following Resource types:
* Practitioner
* PractitionerRole
* Organization

### Logical Model
The diagram below shows how the linked FHIR resources that represent the association of the professional with an organization via a professional role that effectively represents the employment contract.
<br />
{{render:Diagrams-xxxxx}}
<br />

### Message Definition
The applicable message definition can be retrieved via the link below:
* {{pagelink:MessageDefinition/xxx, text: xxxx}}

### Example Bundle
The incorporation of the applicable message header and the required resources are illusted in the example bundle below:
* {{pagelink:Example-DataStandardsWales-Bundle-xxx, text: Example Bundle xxx}}
<br />
# FHIR Messaging Examples
The examples below are illustrative only. They do not represent actual message definitions or event codes in current use by the CDR. They are designed to expose the alternative methods of message construction.

## Example Message Event - Submit Clinician
This example illustrates a possible update of the CDR by a health board to add a new clinician.  The key details are as follows:<br />
><sup>_Clinician:_ Dr Dhiren Patel (nadex:dh000567; GMC:9630333)</sup><br />
><sup>_Health Board:_ Swansea Bay University Health Board</sup><br />
><sup>_Employed as:_ Consultant in Geriatric Medicine</sup><br />

An example {{pagelink:Example-DataStandardsWales-MessageDefinition-SubmitClinician, text:message definition}} has been drawn up for a message event "submit-clinician", to illustrate how the submission could be constrained to include one of each of the following resources:
* {{pagelink:DataStandardsWales-PractitionerRole,text:Practitioner}}
* {{pagelink:DataStandardsWales-PractitionerRole,text:PractitionerRole}}
* {{pagelink:DataStandardsWales-PractitionerRole,text:Organization}}

### Scenario 1. Only Logical Identifiers Available
In this scenario, the source system for the submission has no knowledge of existing FHIR resource identifiers.  Generated literal object identifiers are used within the message to allow the association of each MessageHeader.focus.reference with the corresponding Bundle.entry.fullUrl and the associated resource details, populated as fully as possible.

The bundle construction is illustrated below:
<br />
{{render:Diagrams-FHIR-Example-SubmitClinician-Logical}}
<br />

Example message bundle: {{pagelink:Example-DataStandardsWales-Bundle-SubmitClinician-Logical, text: Example Message Bundle - Submit Clinician (Logical referencing)}}

Prior to creating the new PractitionerRole, the applicable message handler would resolve the logical identfiers for Organization and Practitioner and references and replace the practitioner and organization references within the PractitionerRole resource with literal references to FHIR resources.

### Scenario 2. Literal Referencing of FHIR Resources
In this scenario, the source system for the submission has access to the details of existing FHIR resources and is specifying a new PractitionerRole for an existing Practitioner and Organization. It uses FHIR resource IDs as the MessageHeader.focus.reference for the pre-existing Practitioner and Organization and omits the corresponding Practitioner and Organization bundle entries. The bundle entry for the new PractitionerRole resource also directly references the existing FHIR Practitioner and Organization resources.

The bundle construction is illustrated below:
<br />
{{render:Diagrams-FHIR-Example-SubmitClinician-Literal}}
<br />

Example message bundle: {{pagelink:Example-DataStandardsWales-Bundle-SubmitClinician-Literal, text: Example Message Bundle - Submit Clinician (Literal FHIR referencing)}}

In this case the message handler would need to validate the FHIR practitioner and organization resource references before creating the PractitionerRole.
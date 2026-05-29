### {{page-title}}
The following naming convention applies to the message event code as used by `MessageDefinition.eventCoding` and `MessageHeader.eventCoding`.

The **event** code should be lower case and follow the [kebab-case](https://developer.mozilla.org/en-US/docs/Glossary/Kebab_case) naming convention e.g.  

    ✅ patient-admission-submit  
    ❌ patientAdmission-submit  
    ❌ PatientAdmissionSubmit  

Event codes should be short and descriptive in the form **[primary-content]-[qualifier]-[verb]**
* `primary-content` → a high level description of the content in plain English and hyphenated (e.g. care-document, allergy-list, clinician)
* `qualifier` → optional detail (e.g. initial, amendment, discharge, lab)
* `verb` → action. Common verbs:
    * -submit: request to update if found, else create new.
    * -notify: informational event (server processes but does not persist resources).
    * -cancel: request to revoke/withdraw a prior submission.
    * -update: explicit update only (do not create if missing).
<br>
Avoid acronyms or local system jargon in the event code. Use standard healthcare terms wherever possible. 

Examples **WITHOUT** qualifiers
* observation-submit
* allergy-list-update
* lab-result-notify

Examples **WITH** qualifiers
* observation-lab-submit
* observation-vitalsigns-update
<br>

Representation in event coding element:
```json
"eventCoding": { 
"system": "https://fhir.nhs.wales/CodeSystem/DataStandardsWales-MessageEvent", 
"code": "care-document-submit",
"display": "Care Document Submit"
} 
```
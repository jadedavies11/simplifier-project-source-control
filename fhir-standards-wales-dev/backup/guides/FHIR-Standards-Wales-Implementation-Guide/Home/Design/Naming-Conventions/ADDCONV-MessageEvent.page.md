<span style="font-size: 0.9em;">The following naming convention applies to the message event code as used by `MessageDefinition.eventCoding` and `MessageHeader.eventCoding`.</span>

The **event** code should be lower case and follow the [kebab-case](https://developer.mozilla.org/en-US/docs/Glossary/Kebab_case) naming convention e.g.  

    ✅ patient-admission-submit  
    ❌ patientAdmission-submit  
    ❌ PatientAdmissionSubmit  

Event codes should be short and descriptive in the form **[primary-content]-[qualifier]-[verb]**
* <span style="font-size: 0.9em;"> `primary-content` → a high level description of the content in plain English and hyphenated (e.g. care-document, allergy-list, clinician)</span>
* <span style="font-size: 0.9em;"> `qualifier` → optional detail (e.g. initial, amendment, discharge, lab)</span>
* <span style="font-size: 0.9em;"> `verb` → action. Common verbs:</span>
    * <span style="font-size: 0.9em;"> -submit: request to update if found, else create new.</span>
    * <span style="font-size: 0.9em;"> -notify: informational event (server processes but does not persist resources).</span>
    * <span style="font-size: 0.9em;"> -cancel: request to revoke/withdraw a prior submission.</span>
    * <span style="font-size: 0.9em;"> -update: explicit update only (do not create if missing).</span>
<div style="font-size: 0.9em;">
Avoid acronyms or local system jargon in the event code. Use standard healthcare terms wherever possible.</div><br> 

Examples **WITHOUT** qualifiers
* <span style="font-size: 0.9em;"> observation-submit</span>
* <span style="font-size: 0.9em;"> allergy-list-update</span>
* <span style="font-size: 0.9em;"> lab-result-notify</span>

Examples **WITH** qualifiers
* <span style="font-size: 0.9em;"> observation-lab-submit</span>
* <span style="font-size: 0.9em;"> observation-vitalsigns-update</span>
<br>

Representation in event coding element:
```json
"eventCoding": { 
"system": "https://fhir.nhs.wales/CodeSystem/DataStandardsWales-MessageEvent", 
"code": "care-document-submit",
"display": "Care Document Submit"
} 
```

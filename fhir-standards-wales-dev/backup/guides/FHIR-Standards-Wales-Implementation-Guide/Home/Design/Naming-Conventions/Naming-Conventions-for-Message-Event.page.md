### {{page-title}}
The following naming convention applies to the FHIR Message Event:

The **event** name should be lower case and follow the [kebab-case](https://developer.mozilla.org/en-US/docs/Glossary/Kebab_case) naming convention e.g.  

    ✅ patient-admission-submit  
    ❌ patientAdmission-submit  
    ❌ PatientAdmissionSubmit  

* Event codes should be short and descriptive. 
* Use a verb as a suffix to clarify intent and make it action-oriented.
    * Common verbs: -submit, -notify, -cancel, -update.
<br>

#### Message Event Semantics
* -submit: request to update if found, else create new.
* -notify: informational event (server processes but does not persist resources).
* -cancel: request to revoke/withdraw a prior submission.
* -update: explicit update only (no create if missing).

<br>

#### Message Event Structure
Format: 
`primary-content`-`qualifier`-`verb`
* `primary-content` → a match of the FHIR resource in plain English and hyphenated 
    * DocumentReference → care-document
    * AllergyIntolerance → allergy-list
    * Practitioner → clinician
* `qualifier` → optional detail (e.g. initial, amendment, discharge, lab)
* `verb` → action (e.g. submit, notify, cancel)

Avoid acronyms or local system jargon in the event code. Use standard healthcare terms wherever possible. 

Example **WITHOUT** qualifiers
* observation-submit

Examples **WITH** qualifiers
* observation-lab-submit
* observation-vitalsigns-update
* lab-result-notify

<br>

#### Examples in context 

Event Code: `care-document-submit`

Appears in:  
```json
"eventCoding": { 
"system": "https://fhir.nhs.wales/CodeSystem/message-events", 
"code": "care-document-submit",
"display": "Care Document Submit"
} 
```
Event Code: `observation-lab-result-notify` 

Appears in: 
```json
"eventCoding": {
  "system": "https://fhir.nhs.wales/CodeSystem/message-events",
  "code": "observation-lab-result-notify",
  "display": "Observation Lab Result Notify"
}
```
<br>
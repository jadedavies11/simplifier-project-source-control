## {{page-title}}

The following naming convention applies to the FHIR Message Definition resource defined in this guide:

The **name** of the Message Definition which will follow the [camelCase](https://en.wikipedia.org/wiki/Camel_case) naming convention and use only alphanumeric values.  E.g.
* PatientAdmission
* MedicationDispenseNotification

The following naming convention applies more espefically to the MessageDefinition.event: 

### General Rules
* Use lowercase and using the [kebab-case](https://developer.mozilla.org/en-US/docs/Glossary/Kebab_case) naming convention. E.g.
✅ clinical-document-new
❌ clinicalDocument-new
❌ ClinicalDocumentNew

* Event codes should be short, descriptive, and action-oriented. 
* Suffix with a verb to clarify intent.
    * Common verbs: -new, -notify, -cancel, -update.

### Semantics
* -new: request to create a new event.
* -notify: informational event (server processes but does not persist resources).
* -cancel: request to revoke/withdraw a prior submission. 
* -update: explicit update only (no create if missing). 

### Structure
Format
<primary-resource>-<qualifier>-<verb>
* <primary-resource> -- main FHIR resource (e.g. patient, ServiceRequest, allergy-list)
* <qualifier> -- optional detail (e.g. initial, amendment, discharge)
* <verb> -- action (e.g. new, update, cancel)

### Alignment with FHIR 
Match the FHIR resource name in plain English, hyphenated.
* DocumentReference → clinical-document 
* AllergyIntolerance → allergy-list 
* Practitioner → clinician 
Avoid acronyms or local system jargon in the event code. Use standard healthcare terms wherever possible. 


### Examples
* appointment-cancel
* patient-contact-update
* emergency-care-arrival-new
* lab-result-notify

* Examples in Context 
Event Code: clinical-document-new
Appears in: 
"eventCoding": { 
"system": "https://fhir.nhs.wales/CodeSystem/message-events", 
"code": "clinical-document-new", 
"display": "New Clinical Document"} 



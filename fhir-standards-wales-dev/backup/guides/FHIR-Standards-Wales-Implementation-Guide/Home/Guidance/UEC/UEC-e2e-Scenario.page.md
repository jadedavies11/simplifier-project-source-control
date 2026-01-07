## UEC End-to-End Scenario
### Scenario Overview
This scenario covers the attendance of a patient at a minor injuries facilty with a swollen ankle, from the point of arrival through to the discharge of the patient back to her home.

The required data submissions for this scenario are illustrated in the sections below for the three distinct message events. As the UEC application has no knowledge of the FHIR resources created by the prior submissions, the data sent will be cumulative. The relevant data from the prior step(s) will be resubmitted to ensure that all of the links can be fully resolved by the CDR message handler.

NOTE that any investigations, the problem list (formal diagnoses), problem management, the discharge information document and follow up are beyond the scope of the Phase 1 UEC data submissions.

### Step 1 - UEC Arrival
{{page:Step-1-UEC-Arrival}}

### Step 2 - UEC Triage
{{page:Step-2-UEC-Triage}}

### Step 3 - UEC Discharge
{{page:Step-3-UEC-Discharge}}
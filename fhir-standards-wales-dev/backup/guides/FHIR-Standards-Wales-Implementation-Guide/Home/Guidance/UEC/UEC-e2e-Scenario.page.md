## UEC End-to-End Scenario
Ms Marjorie Pryor attends the Emergency Unit Minor Injuries facility of University Hospital of Wales at 12:00 on 02/12/2025 with a painful swollen ankle. She has been advised to attend by her GP at North Cardiff Medical Centre and an appointment was booked for 12:15. She travelled to the appointment by bus.  This was her first UEC attendance for the condition.

At 12:12 she was assessed by triage nurse Mrs Lisa Potts as requiring standard level emergency care acuity and the swollen ankle was recorded together with the comorbidities of asthma and hypertension. 

Marjorie was seen by a health care support worker and a consultant during the visit, the first at 12:30.  The consultations resulted in a diagnosis of a sprained ankle and appropriate management, before Marjorie was discharged to home at 14:35, with advice for follow-up via her general practitioner. A copy of the discharge letter was provided to her at the point of discharge.

NOTE that any investigations, the problem list (formal diagnoses), problem management, the discharge information and follow up are beyond the scope of the Phase 1 UEC data submissions.

### Step 1 - UEC Arrival
The first data submission occurs after the patient arrival at the UEC facility has been registered.  The case-specific details known at this stage are:
><sup>_Patient identity:_ Ms Marjorie Pryor (CAV PAS Number A272114; NHS number not present)</sup><br />
><sup>_Patient address:_ 7 Llandaff Court, Penarth CF64 3JH</sup><br />
><sup>_Patient birth date:_ 1961-12-16</sup><br />
><sup>_Patient gender:_ Female</sup><br />
><sup>_Patient ethnic category:_ Any White Background, including Welsh, English, Scottish, Northern Irish, Irish, British</sup><br />
><sup>_Patient LHB of residence:_ Cardiff and Vale University Health Board</sup><br />
><sup>_Patient registered GP practice:_ North Cardiff Medical Centre</sup><br />
><sup>_Encounter UEC activity identifier:_ 123456789</sup><br />
><sup>_Encounter expected time of treatment:_ 2025-12-02 12:15</sup><br />
><sup>_Encounter mode of arrival:_ Public transport / taxi</sup><br />
><sup>_Encounter attendance category:_ Unplanned first Urgent and Emergency Care or Same Day Emergency Care Attendance for a new clinical condition (or deterioration of a chronic condition).</sup><br />
><sup>_Encounter activity type:_ Emergency Care Attendance at an Emergency Care Department Type Minor Injury Unit.</sup><br />
><sup>_Encounter care consultation mechanism:_ Face to face</sup><br />
><sup>_Encounter activity start time:_ 2025-12-02 12:00</sup><br />
><sup>_Encounter activity source:_ Referred by member of Primary Health Care Team</sup><br />
><sup>_Encounter activity source organisation:_ North Cardiff Medical Centre</sup><br />
><sup>_Encounter location (UEC facility):_ UHW Emergency Unit Minor Injuries, managed by University Hospital of Wales</sup><br />
><sup>_Encounter service provider:_ Cardiff and Vale University Health Board</sup><br />

There are also some fixed values that will provide context within the FHIR Encounter resource:
><sup>_Encounter class:_ emergency</sup><br />
><sup>_Encounter status:_ arrived</sup><br />
><sup>_Encounter service type:_ Emergency medicine service</sup><br />

The bundle construction for this step is illustrated below, together with a populated example message bundle.
<br />
{{render:Diagrams-UEC-arrival-messaging-model}}
<br />

Message bundle: {{pagelink:Example-DataStandardsWales-Bundle-UEC-Arrival-UHWEUMI, text: Example Message Bundle - UEC Arrival UHWEUMI (UHW Emergency Unit Minor Injuries)}}
Message definition: {{pagelink:MessageDefinition-DataStandardsWales-UEC-Arrival}}

### Step 2 - UEC Triage
The second data submission occurs after the patient has been triaged at the UEC facility and the acuity of the attendance determined. In order to create the new version of the Encounter reasource, the message handler will require all of the details supplied above that are still valid.  The additional case-specific details known at this stage are:
><sup>_Encounter acuity:_ 4 - Standard level emergency care</sup><br />
><sup>_Encounter chief complaint:_ Swollen ankle (267039000)</sup><br />
><sup>_Encounter comorbidities:_ Asthma (195967001); Hypertension (38341003)</sup><br />
><sup>_Encounter participant (triage nurse):_ Mrs Lisa Potts (NMC:AB123456W) as nurse for CAVUHB</sup><br />

The status and status history will need to be updated:
><sup>_Encounter status:_ triaged</sup><br />
><sup>_Encounter statusHistory:_ arrived start 2025-12-02 12:00 end 2025-12-02 12:11:59</sup><br />

The bundle construction for this step is illustrated below, together with a populated example message bundle.
<br />
{{render:Diagrams-UEC-triage-messaging-model}}
<br />

Message bundle: {{pagelink:Example-DataStandardsWales-Bundle-UEC-Triage-UHWEUMI, text: Example Message Bundle - UEC Triage UHWEUMI (UHW Emergency Unit Minor Injuries)}}
Message definition: {{pagelink:MessageDefinition-DataStandardsWales-UEC-Triage}}

### Step 3 - UEC Discharge
The final data submission occurs after the patient has been discharged at the UEC facility. The additional case-specific details known at this stage are:
><sup>_Encounter participant:_ Mark Smith (NADEX: ma000199) as health care support worker for CAVUHB</sup><br />
><sup>_Encounter participant:_ Dr Dhiren Patel (nadex:dh000567; GMC:9630333) as consultant in geriatric medicine for CAVUHB</sup><br />
><sup>_Encounter discharge status:_ Treatment complete</sup><br />
><sup>_Encounter discharge destination:_ Discharge to home</sup><br />
><sup>_Encounter discharge information given:_ A copy of the discharge letter was given to the patient</sup><br />

The status and status history will need to be updated to include the current status and all prior statuses:
><sup>_Encounter status:_ finished</sup><br />
><sup>_Encounter statusHistory:_ arrived start 2025-12-02 12:00 end 2025-12-02 12:11:59</sup><br />
><sup>_Encounter statusHistory:_ triaged start 2025-12-02 12:12 end 2025-12-02 12:29:59</sup><br />
><sup>_Encounter statusHistory:_ in-progress start 2025-12-02 12:30 end 2025-12-02 14:34:59</sup><br />

The bundle construction for this step is illustrated below, together with a populated example message bundle.
<br />
{{render:Diagrams-UEC-discharge-messaging-model}}
<br />

Message bundle: {{pagelink:Example-DataStandardsWales-Bundle-UEC-Discharge-UHWEUMI, text: Example Message Bundle - UEC Discharge UHWEUMI (UHW Emergency Unit Minor Injuries)}}
Message definition: {{pagelink:MessageDefinition-DataStandardsWales-UEC-Discharge}}
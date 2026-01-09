## {{page-title}}

Placeholder content.  Guidance to be developed shortly.

### Data Model Overview
<br />
{{render:Diagrams-UEC-encounter-maximal-logical-model}}
<br />

### FHIR Resources
* {{pagelink:DataStandardsWales-Condition}}
* {{pagelink:DataStandardsWales-Device}}
* {{pagelink:DataStandardsWales-DocumentReference}}
* {{pagelink:DataStandardsWales-Encounter-UEC}}
* {{pagelink:DataStandardsWales-Location}}
* {{pagelink:DataStandardsWales-Organization}}
* {{pagelink:DataStandardsWales-Patient}}
* {{pagelink:DataStandardsWales-PractitionerRole}}
* {{pagelink:DataStandardsWales-Provenance}}

### FHIR Messaging Resources
* [Bundle](https://www.hl7.org/fhir/R4/bundle.html)
* {{pagelink:DataStandardsWales-MessageDefinition}}
* {{pagelink:DataStandardsWales-MessageHeader}}

### UEC Message Definitions
* {{pagelink:MessageDefinition-DataStandardsWales-UEC-Arrival}}

### Data Standards Wales Value Sets used in UEC Arrival Messaging
* {{pagelink:ValueSet-DataStandardsWales-MessageEvent, text:ValueSet-DataStandardsWales-MessageEvent}}
* {{pagelink:ValueSet-DataStandardsWales-UEC-Acuity, text:ValueSet-DataStandardsWales-UEC-Acuity}}
* {{pagelink:ValueSet-DataStandardsWales-UEC-ArrivalMode, text:ValueSet-DataStandardsWales-UEC-ArrivalMode}}
* {{pagelink:ValueSet-DataStandardsWales-UEC-AttendanceCategory, text:ValueSet-DataStandardsWales-UEC-AttendanceCategory}}
* {{pagelink:ValueSet-DataStandardsWales-UEC-AttendanceSource, text:ValueSet-DataStandardsWales-UEC-AttendanceSource}}
* {{pagelink:ValueSet-DataStandardsWales-UEC-DischargeDestination, text:ValueSet-DataStandardsWales-UEC-DischargeDestination}}

### Data Standards Wales Code Systems used in UEC Arrival Messaging
* {{pagelink:CodeSystem-DataStandardsWales-UEC-ActivityType, text:CodeSystem-DataStandardsWales-UEC-ActivityType}}
* {{pagelink:CodeSystem-DataStandardsWales-UEC-AttendanceCategory, text:CodeSystem-DataStandardsWales-UEC-AttendanceCategory}}
* {{pagelink:CodeSystem-DataStandardsWales-UEC-CareConsultationMechanism, text:CodeSystem-DataStandardsWales-UEC-CareConsultationMechanism}}
* {{pagelink:CodeSystem-DataStandardsWales-UEC-MessageEvent, text:CodeSystem-DataStandardsWales-UEC-MessageEvent}}

### Generic Messaging Model Structure - UEC Arrival
<br />
{{render:Diagrams-UEC-arrival-messaging-model}}
<br />

### Example Message Bundle for UEC Arrival
Scenario: Ms Marjorie Pryor (CAV PAS Number A272114) attends the Emergency Unit Minor Injuries facility of University Hospital of Wales at 12:00 on 02/12/2025.  She has been advised to attend by her GP at North Cardiff Medical Centre and an appointment was booked for 12:15. She travelled to the appointment on public transport.  This was her first UEC attendance for the condition.

Message bundle: 
* {{pagelink:Example-DataStandardsWales-Bundle-UEC-Arrival-UHWEUMI, text: Example Message Bundle - UEC Arrival UHWEUMI (UHW Emergency Unit Minor Injuries)}}
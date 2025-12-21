# Urgent and Emergency Care
<div style="float:right;border:1px;border-style:solid;padding:10px;margin:10px;width:300px;">

  - [Introduction](#introduction)
  - [Data Model Overview](#data-model-overview)
  - [FHIR Resources](#fhir-resources)
    * [Condition](#condition)
    * [Device](#device)
    * [Encounter-UEC](#encounter-uec)
    * [Location](#location)
    * [Organization](#organization)
    * [Patient](#patient)
    * [PractitionerRole](#practitionerrole)
    * [Provenance](#provenance)
  - [Submission of UEC data to the CDR](#submission-of-uec-data-to-the-cdr)
    * [FHIR Messaging Resources](#fhir-messaging-resources)
    * [UEC Message Events](#uec-message-events)
    * [UEC Message Definitions](#uec-message-definitions)
    * [Encounter-UEC](#encounter-uec)
  - [UEC End-to-End Scenario](#uec-end-to-end-scenario)
    * [Step 1 - UEC Arrival](#step-1-uec-arrival)
    * [Step 2 - UEC Triage](#step-2-uec-triage)
    * [Step 3 - UEC Discharge](#step-3-uec-discharge)
 
</div>

## Introduction
The Welsh Emergency Care Data Set (WECDS) defines the data required from new Urgent and Emergency Care (UEC) applications.  A phased approach is being taken to supporting the capture of UEC data within the Care Data Repository (CDR). The scope of the current (first) phase is the submission of UEC activity data relating to the arrival of a patient at an Urgent and Emergency Care (UEC) facility, their initial assessment (triage) and their discharge and departure from the facility. The data will be made available via the National Data Analytics Platform for secondary analysis of UEC facility utilisation.

A specific resource profile has been developed for a UEC encounter.  This includes with dedicated extensions, value sets and code systems to support the relevant data requirements.  As explicit support for data submission to the CDR, candidate message events, message definition instances and example data bundles are also provided within this implementation guide.

## Data Model Overview
The UEC data for each patient attendance will be stored as a dedicated UEC Encounter resource linked to Condition resources for the chief complaint and any comorbidies noted during the attendance. The attendance context and involved clinicial staff will be captured through linking of the applicable FHIR administrative resources such as Organization, Location and PractitionerRole. The creation or update of a UEC Encounter or Condition will be associated with one or more Provenance instances, targeting the specific resource versions created. 

The diagram below provides an overview of the involved FHIR resources and how they can be interconnected to support the relevant subset of the WECDS. The presence or absence of certain links will depend upon the specific use case and the progress through the UEC encounter.

The FHIR data model consists of the following resources: 
* {{pagelink:DataStandardsWales-Condition, text:Condition}}
* {{pagelink:DataStandardsWales-Device, text:Device}}
* {{pagelink:DataStandardsWales-Encounter-UEC, text:Encounter-UEC}}
* {{pagelink:DataStandardsWales-Location, text:Location}}
* {{pagelink:DataStandardsWales-Organization}}
* {{pagelink:DataStandardsWales-Patient}}
* {{pagelink:DataStandardsWales-PractitionerRole}}
* {{pagelink:DataStandardsWales-Provenance}}

<br />
{{render:Diagrams-UEC-encounter-maximal-logical-model}}
<br />

### Condition
The Condition resource should be used to capture both the chief complaint for the UEC attendance and any comorbidities recorded during the attendance.

### Device
The Device resource represents the systems from which the UEC data submission was sourced.

### Encounter-UEC
The UEC Encounter profile is a specialisation of the standard Encounter resource which should be used to represent the attendance of the patient at the UEC facility, from the time of arrival to the time of departure.  It makes use of the following UEC-specific value sets:
* {{pagelink:ValueSet-DataStandardsWales-UEC-Acuity}}
* {{pagelink:ValueSet-DataStandardsWales-UEC-ArrivalMode}}
* {{pagelink:ValueSet-DataStandardsWales-UEC-AttendanceCategory}}
* {{pagelink:ValueSet-DataStandardsWales-UEC-AttendanceSource}}
* {{pagelink:ValueSet-DataStandardsWales-UEC-DischargeDestination}}

### Location
A Location resource is referenced to identify the specific UEC facility (e.g. a specific minor injuries department) that the patient attended for the UEC encounter.

### Organization
One or more Organization resources may be referenced from the encounter to identify the service provider (typically a Health Board) that is responsible for the UEC encounter, the organization that manages the UEC facility and, where applicable, the source organisation and the organisation to which the patient is discharged. Where different from the service provider, the following organisations may also be involved:
- The patient's health board of residence (referenced from the Patient resource)
- The health board employer of a participant (referenced from the PractitionerRole resource)

### Patient
A Patient resource is referenced to identify the attendee at the UEC facility i.e. the subject of the UEC encounter.

### PractitionerRole
A PractitionerRole resource is referenced to identify each UEC care professional involved with the patient during their UEC attendance, including their specialty and the health board under which they were operating.  

### Provenance
The Provenance resource will capture metadata related to the creation or update of each affected resource instance (as the target of the provenance record) and may also be used to capture the subject demographics at the time of the encounter. Provenance content will be specifically determined and the appropriate instances assembled by the CDR message handler, so it will not appear within the submission message examples in the section below.

See the dedicated guidance page for clarification of the purpose and use of the Provenance resource: {{pagelink:Home/Guidance/Provenance/Index.page.md, text: Provenance Guidance}}

## Submission of UEC data to the CDR
### FHIR Messaging Resources
Submissions of UEC data from UEC applications to the CDR will use the FHIR messaging paradigm and the following FHIR messaging resources:
* [Bundle](https://www.hl7.org/fhir/R4/bundle.html) 
* {{pagelink:DataStandardsWales-MessageDefinition, text:MessageDefinition}}
* {{pagelink:DataStandardsWales-MessageHeader, text:MessageHeader}}

The following resource will be used within the response bundle to convey any issues encountered by the CDR message handler:
* [OperationOutcome](https://www.hl7.org/fhir/R4/operationoutcome.html)

See the dedicated guidance page for clarification of the purpose and use of the resources involved in FHIR messaging: {{pagelink:Home/Guidance/FHIR-Messaging/Index.page.md, text: FHIR Messaging Guidance}}

### UEC Message Events
The following message events have been defined FOR TRIAL USE at Phase 1, pending the establishment of a naming convention for message events.

| Message event | Submission point             | Resources (if applicable to use case)           |
|:--|:--|:------|
| uec-arrival<br /><br /><br /><br /><br /> | On completion of registering the <br />patient’s arrival at the UEC facility<br /><br /><br /> <br />| Encounter-UEC <br />Patient<br />Organization (service provider)<br />Organization (attendance source)<br />Location (UEC facility) |
| uec-triage<br /><br /><br /><br /><br /><br /><br /><br /> | On completion of recording the <br />triage assessment<br /><br /><br /> <br /><br /><br /><br />| Encounter-UEC <br />Patient<br />Organization (service provider)<br />Organization (attendance source)<br />Location (UEC facility)<br />ProfessionalRole (e.g. triage nurse)<br />Condition (chief complaint)<br />Condition (each comorbidity) |
| uec-discharge<br /><br /><br /><br /><br /><br /><br /><br /><br /> | On completion of the UEC attendance <br />i.e. the point of discharge<br /><br /><br /><br /><br /><br /><br /><br />| Encounter-UEC <br />Patient<br />Organization (service provider)<br />Organization (attendance source)<br />Location (UEC facility)<br />ProfessionalRole (each professional)<br />Condition (chief complaint)<br />Condition (each comorbidity)<br />DocumentReference (discharge information) |

These message events have been captured in a dedicated code system that can be extended as the scope increases through the project phases:
* {{pagelink:CodeSystem-DataStandardsWales-UEC-MessageEvent}}

### UEC Message Definitions
MessageDefinition resource instances have been defined FOR TRIAL USE for the Phase 1 UEC data submissions
* {{pagelink:MessageDefinition-DataStandardsWales-UEC-Arrival}}
* {{pagelink:MessageDefinition-DataStandardsWales-UEC-Triage}}
* {{pagelink:MessageDefinition-DataStandardsWales-UEC-Discharge}}

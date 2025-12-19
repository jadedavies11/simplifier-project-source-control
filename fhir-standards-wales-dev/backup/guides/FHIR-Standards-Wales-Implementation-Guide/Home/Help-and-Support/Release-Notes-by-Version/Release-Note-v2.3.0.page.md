## {{page-title}}

Package: 
* {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions,text:Profiles and Extensions}}:
    * New Profiles
        * DataStandardsWales-Composition
        * DataStandardsWales-Condition        
        * DataStandardsWales-Consent
        * DataStandardsWales-DocumentReference
        * DataStandardsWales-Encounter-UEC
        * DataStandardsWales-ImmunizationRecommendation
    * New Extensions
        * DataStandardsWales-AdministeredProduct
        * DataStandardsWales-DateProcedureLastUpdated        
        * DataStandardsWales-DocumentAttribute
        * DataStandardsWales-DocumentDigitalStatus
        * DataStandardsWales-DocumentErrorAction
        * DataStandardsWales-DocumentErrorStatus
        * DataStandardsWales-ForecastCreationSource
        * DataStandardsWales-SourceSystem
        * DataStandardsWales-UECAttendanceCategory
        * DataStandardsWales-UECDischargeInformationGiven
        * DataStandardsWales-UECExpectedTimeOfTreatment
    * New R5 backport Extensions:      
        * DataStandardsWales-DocumentAttester
        * DataStandardsWales-DocumentVersion
        * DataStandardsWales-Immunization.basedOn
    * Changes to Profiles
        * DataStandardsWales-Appointment
            * Updated version from 1.0.0 to 1.0.1
            * .reasonReference. Added reference to DataStandardsWales-ImmunizationRecommendation
        * DataStandardsWales-DiagnosticReport
            * Updated version from 0.1.1 to 0.1.2
            * .basedOn. Added reference to DataStandardsWales-ImmunizationRecommendation
        * DataStandardsWales-DiagnosticReport-Lab
            * Updated version from 0.1.0 to 0.1.1
            * .basedOn. Added reference to DataStandardsWales-ImmunizationRecommendation
        * DataStandardsWales-Encounter
            * Updated version from 1.0.0 to 1.0.1
            * .appointment. Added reference to DataStandardsWales-Appointment
            * .reasonReference. Added reference to DataStandardsWales-ImmunizationRecommendation
            * .serviceProvider. Added Must Support flag.
        * DataStandardsWales-ImagingStudy
            * Updated version from 0.0.6 to 0.0.7
            * .basedOn. Added reference to DataStandardsWales-Appointment
        * DataStandardsWales-Immunization
            * Updated version from 0.1.1 to 1.0.0
            * Updated status from draft to active
            * Removed experimental flag
            * New extensions added:
                * DataStandardsWales-AdministeredProduct
                * DataStandardsWales-DateProcedureLastUpdated
                * DataStandardsWales-ForecastCreationSource
                * DataStandardsWales-Immunization.basedOn
            * R5 backport extension:
                * DataStandardsWales-Immunization.basedOn
            * Terminology binding changes:
                * .protocolApplied.targetDisease. ValueSet reverted to UK Core STU2 so changed from covid-19-diseases to immunization-target-disease
            * Binding strength changes:
                * .protocolApplied.targetDisease. From required to example
            * .basedOn. Added reference to DataStandardsWales-ImmunizationRecommendation
        * DataStandardsWales-MedicationRequest
            * Updated version from 1.1.1 to 1.1.2
            * .basedOn. Added reference to DataStandardsWales-ImmunizationRecommendation
        * DataStandardsWales-Observation
            * Updated version from 0.1.1 to 0.1.2
            * .basedOn. Added reference to DataStandardsWales-ImmunizationRecommendation
            * .reasonReference. Added reference to DataStandardsWales-ImmunizationRecommendation
        * DataStandardsWales-Practitioner
            * Updated version from 1.1.2 to 1.1.3
            * Cardinality changes:
                * identifier:nadexIdentifier. From 0..1 to 0..* 
        * DataStandardsWales-PractitionerRole
            * Updated version from 1.1.1 to 1.1.2
            * .specialty. Changed valueset binding from required to extensible to align with UK Core
* {{pagelink:Home/FHIR-Assets/Terminology,text:Terminology}}:
    * New Value Sets 
        * Data Standards Wales Document Category
        * Data Standards Wales Document Digital Status
        * Data Standards Wales Document Type
        * Data Standards Wales Encounter Type 
        * Data Standards Wales UEC Activity Type
        * Data Standards Wales UEC Acuity
        * Data Standards Wales UEC Arrival Mode
        * Data Standards Wales UEC Attendance Category
        * Data Standards Wales UEC Attendance Source
        * Data Standards Wales UEC Care Consultation Mechanism
        * Data Standards Wales UEC Discharge Destination
        * FHIR Standards Wales Document Attribute
        * FHIR Standards Wales Document Error Action
        * FHIR Standards Wales Document Error Status
        * PAS Event Type
    * New Code Systems
        * Data Standards Wales Document Category
        * Data Standards Wales Document Digital Status
        * Data Standards Wales UEC Activity Type
        * Data Standards Wales UEC Attendance Category
        * Data Standards Wales UEC Care Consultation Mechanism
        * FHIR Standards Wales Document Attribute
        * FHIR Standards Wales Document Error Action
        * FHIR Standards Wales Document Error Status
        * WPAS Event Type
* {{pagelink:Home/FHIR-Assets/Naming-Systems.page.md,text:Naming Systems}}
    * Changes to Naming Systems
        * Namespaces for PAS Appointment ids
            * Updated value from pas-event-code to pas-event-identifier
            * Changed name from AppointmentIdentifier to XXXXPASAppointmentIdentifier where XXXX is the healthboard/trust abbreviation
        * New Naming Systems
            * Namespaces for PAS Practitioner id. This is to aid in the mapping of the HL7 v2 messages into FHIR. It is to the capture 'local' identifiers for practitioners where they may not exist in the CDR.
            * Namespaces for LIMS TCLE and TCL system identifiers. This is to aid in the mapping of the HL7 v2 messages into FHIR. It is to the capture 'local' identifiers for LIMS where they may not exist in the CDR. These include LIMS identifiers for procedure, report and specimen type codes.
            * Namespaces for PAS upi identifiers. These additional identifiers are for referrals and appointments and encounters so CDR can identify when an appointment has come from a referral and when a patient has e.g arrived at their appointment.  CDR would store this value as an additional identifier against each referral, appointment and encounter in the existing identifier FHIR array.
            * Namespace for WCRS DocumentId values
            * Namespace for WCRS DocumentSupersessionSetId values
* {{pagelink:Home/Example-Index.page.md,text:Examples}}:
    * New Examples
        * Document Reference
            * {{pagelink:Example-DataStandardsWales-DocumentReference-EncounterBased, text:Encounter-based}}
            * {{pagelink:Example-DataStandardsWales-DocumentReference-EventBased, text: Event-based}}
            * {{pagelink:Example-DataStandardsWales-DocumentReference-NotEventBased, text: Not event-based}}
            * {{pagelink:Example-DataStandardsWales-DocumentReference-MisfiledNotEventBased, text: Misfiled (document not event-based)}}

Guide:
* General improvements to IG that include fixing spelling mistakes and correcting grammatical errors
* Added a new page to outline the DataStandardsWales-Consent profile
* Added a new page to outline the DataStandardsWales-Condition profile
* Added a new page to outline the DataStandardsWales-Composition profile
* Added a new page to outline the DataStandardsWales-Encounter-UEC profile
* Added a new page to outline the DataStandardsWales-ImmunizationRecommendation profile
* Added a new page to outline the DataStandardsWales-DocumentReference profile
* Added new pages to outline the Data Standards Wales Extensions created in this release
* Added new pages to outline the Data Standards Wales Value Sets created in this release
* Added new pages to outline the Data Standards Wales Code Systems created in this release
* Added new pages to outline the Data Standards Wales Examples created in this release
* Removed DataStandardsWales-Dosage profile from main index
* Removed NHS Wales Identity Provider User ID (also known as Nadex) section from Naming Systems page
* Added Health Board PAS names to AppointmentIdentifier Name in Naming Systems table
* Updated Provenance Guidance page
* Moved DataStandardsWales-Device from Diagnostics to Entities in Resource Index page
* Added HL7 International R4 tile to Related Pages
* Added HL7 International R5 tile to Related Pages
* Added namespaces for WCRS DocumentId and WCRS DocumentSupersessionSetId values in Naming Systems table
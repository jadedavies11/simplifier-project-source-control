## {{page-title}}

### v2.5.0 STU2
Package: 
* {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions,text:Profiles and Extensions}}:
    * New Profiles
        * DataStandardsWales-MessageDefinition
        * DataStandardsWales-MessageHeader
    * New Extensions 
    * New Message Definitions
        * MessageDefinition-DataStandardsWales-UEC-Arrival
    * Changes to Profiles
        * DataStandardsWales-MedicationRequest
            * Updated version from 1.2.0 to 1.3.0
            * .requestor. Cardinality changed from 1..1 to 0..1 to align with UKCore.
    * Changes to Extensions
* {{pagelink:Home/FHIR-Assets/Terminology,text:Terminology}}:
    * New Code Systems
        * DataStandardsWales-UEC-MessageEvent
    * Removed Code Systems
    * Changes to Code Systems
    * New Value Sets
        * DataStandardsWales-MessageEvent
    * Removed Value Sets
    * Changes to Value Sets
        * DataStandardsWales-EncounterType
            * Updated version from 1.0.0 to 1.1.0
            * Updated SNOMED CT 20250409 version 
            * Expanded SNOMED CT codes to show 50 concepts as sample
        * DataStandardsWales-Occupation
            * Updated version from 0.0.5 to 0.1.0
            * Updated SNOMED CT 20250409 version 
            * Expanded SNOMED CT codes to show 50 concepts as sample
        * DataStandardsWales-Occupation
            * Updated version from 1.0.0 to 1.1.0
            * Updated SNOMED CT 20250409 version 
            * Expanded SNOMED CT codes to show 50 concepts as sample
* {{pagelink:Home/FHIR-Assets/Naming-Systems.page.md,text:Naming Systems}}
    * Changes to Naming Systems
        * New Naming Systems
            * Namespaces for PAS link identifiers
* {{pagelink:Home/Example-Index.page.md,text:Examples}}:
    * New Examples
        * Urgent and Emergency Care
            * Example Message Bundle - UEC Arrival UHWEUMI (UHW Emergency Unit Minor Injuries)
        * FHIR Messaging guidance
            * Example Message Bundle - Submit Clinician (Logical Referencing)
            * Example Message Bundle - Submit Clinician (Literal FHIR Referencing)
            * Example Message Definition - Submit Clinician

Guide:
* General improvements to IG that include fixing spelling mistakes, correcting grammatical errors and formatting
* Added a new page to outline the DataStandardsWales-MessageDefinition profile
* Added a new page to outline the DataStandardsWales-MessageHeader profile
* Added new pages to outline the Message Definitions created in this release
* Added new pages to outline the Code Systems created in this release
* Added new pages to outline the Value Sets created in this release
* Added new pages to outline the Examples created in this release
* Added FHIR Messaging Guidance page
* Added Urgent and Emergency Care Guidance page (PLACEHOLDER)
* Added WRTS contact details to DataStandardsWales-EncounterType Value Set guide page
* Added WRTS contact details to DataStandardsWales-Occupation Value Set guide page
* Added WRTS contact details to DataStandardsWales-Religion Value Set guide page
* Removed duplicated examples from DataStandardsWales-Observation guide page. All examples are now located in the Examples tab of the Profile Content table
* Renamed Naming Systems page in Design tab to Naming Systems Design
* Updated page link in FHIR Assets Naming System from Naming System to Naming Systems Design
* Standardised resource links in IG pages
* Correct title page for Extension Data Standards Wales Speciality to align with IG standards
* Alphabetised yaml toc files
* Standardised examples names in Example Index page


### v2.4.0 STU2
Package: 
* {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions,text:Profiles and Extensions}}:
    * New Extensions
        * DataStandardsWales-ClinicCode
    * Changes to Profiles
        * DataStandardsWales-Appointment
            * Updated version from 1.0.1 to 1.1.0
            * .basedOn. Updated reference to DataStandardsWales-ImmunizationRecommendation   
            * New extension added:
                * DataStandardsWales-ClinicCode
            * .reasonReference. Added reference to DataStandardsWales-Condition    
        * DataStandardsWales-Consent
            * Updated version from 0.0.1 to 0.0.2
            * .source. Added reference to DataStandardsWales-DocumentReference
        * DataStandardsWales-DiagnosticReport
            * Updated version from 0.1.2 to 0.1.3            
            * .basedOn. Updated reference to DataStandardsWales-ImmunizationRecommendation
        * DataStandardsWales-DiagnosticReport-Lab
            * Updated version from 0.1.1 to 0.1.2            
            * .basedOn. Updated reference to DataStandardsWales-ImmunizationRecommendation
        * DataStandardsWales-Encounter
            * Updated version from 1.0.1 to 1.0.2
            * .condition. Added reference to DataStandardsWales-Condition
            * .reasonReference. Added reference to DataStandardsWales-Condition
            * .basedOn. Updated reference to DataStandardsWales-ImmunizationRecommendation
        * DataStandardsWales-Encounter-UEC
            * Updated version from 0.0.1 to 0.0.2
            * .condition. Added reference to DataStandardsWales-Condition
            * .reasonReference. Added reference to DataStandardsWales-Condition
        * DataStandardsWales-ImagingStudy
            * Updated version from 0.0.7 to 0.1.0
            * .reasonReference. 
                * Added reference to DataStandardsWales-Condition
                * Added reference to DataStandardsWales-DocumentReference
            * .series.specimen. Added reference to DataStandardsWales-Specimen
        * DataStandardsWales-MedicationRequest
            * Updated version from 1.1.2 to 1.2.0
            * .performer. Added reference to DataStandardsWales-RelatedPerson     
            * .basedOn. Updated reference to DataStandardsWales-ImmunizationRecommendation         
        * DataStandardsWales-Observation
            * Updated version from 0.1.2 to 0.1.3
            * .derivedFrom. Added reference to DataStandardsWales-DocumentReference
            * .basedOn. Updated reference to DataStandardsWales-ImmunizationRecommendation
        * DataStandardsWales-Observation-Lab
            * Updated version from 0.1.1 to 0.1.2
            * .hasMember . Added reference to DataStandardsWales-QuestionnaireResponse
        * DataStandardsWales-Observation-VitalSigns-BMI
            * Updated version from 1.1.0 to 1.1.1
            * .note.author. Added reference to DataStandardsWales-RelatedPerson
        * DataStandardsWales-ServiceRequest
            * Updated version from 1.0.0 to 1.0.1
            * .reasonReference. Added reference to DataStandardsWales-DocumentReference
    * Changes to Extensions
        * DataStandardsWales-Immunization.basedOn
            * Updated version from 0.1.0 to 0.1.1
            * value. Added reference to DataStandardsWales-ImmunizationRecommendation
        * DataStandardsWales-UEC-DischargeInformationGiven
            * Updated version from 0.0.1 to 0.0.2
            * dischargeInformation.value. Added reference to DataStandardsWales-DocumentReference
* {{pagelink:Home/FHIR-Assets/Terminology,text:Terminology}}:
    * New Code Systems
        * DataStandardsWales-MainSpecialty
        * MessageEvents
        * WPASReferralSource
        * WPASAdmitSource
        * WPASSourceAdmission
    * Changes to Code Systems
        * FHIR Standards Wales Document Attribute
            * Added display information
    * New Value Sets
        * DataStandardsWales-MainSpecialty
        * MessageEvents
        * PASReferralSource
        * PASAdmitSource
        * PASSourceAdmission
    * Removed Value Sets 
        * DataStandardsWales-UEC-ActivityType
        * DataStandardsWales-UEC-CareConsultationMechanism
    * Changes to Value Sets 
        * DataStandardsWales-DocumentType
            * Updated version from 0.0.1 to 0.0.2
            * Expanded SNOMED CT codes to show 50 concepts as sample
            * Constraint changed from descendantOf to memberOf
        * DataStandardsWales-EncounterType
            * Expanded DataStandardsWales-UEC-CareConsultationMechanism Code System
            * Expanded DataStandardsWales-UEC-ActivityType Code System
        * DataStandardsWales-GenderIdentity
            * Updated version from 1.0.1 to 1.1.0
            * Removed code system version in URI reference
        * DataStandardsWales-MaritalStatus
            * Updated version from 1.0.1 to 1.1.0
            * Removed code system version in URI reference
        * DataStandardsWales-Sex
            * Updated version from 1.0.1 to 1.1.0
            * Removed code system version in URI reference
        * DataStandardsWales-Title
            * Updated version from 1.0.1 to 1.1.0
            * Removed code system version in URI reference
* {{pagelink:Home/FHIR-Assets/Naming-Systems.page.md,text:Naming Systems}}
    * Changes to Naming Systems
        * New Naming Systems
            * Namespace for UEC Attendance Identifier
            * Namespaces for LIMS TCLE and TCL patient identifiers
        * Update to PAS Sub-Specialty Naming Systems
            * Health Board initials prefix added to the Name element

Guide:
* General improvements to IG that include fixing spelling mistakes, correcting grammatical errors and formatting
* Added new pages to outline the Data Standards Wales Extensions created in this release
* Added new pages to outline the Code Systems created in this release
* Added new pages to outline the Value Sets created in this release
* Added Care Documents Guidance page
* Updated resource link on the Guidance: Growth Charts page from Observation to Patient profile
* Added UEC AttendanceIdentifier Name in Naming Systems table
* Removed ValueSet-DataStandardsWales-UEC-ActivityType from Terminology page
* Removed ValueSet-DataStandardsWales-UEC-CareConsultationMechanism from Terminology page
* Added LIMS TCLE and TCL patient identifiers in Naming Systems table
* Added DataStandardsWales-UEC-CareConsultationMechanism Code System to DataStandardsWales-EncounterType Value Set guide page
* Added DataStandardsWales-UEC-ActivityType Code System to DataStandardsWales-EncounterType Value Set guide page
* Added a new page to outline the DataStandardsWales-ClinicCode extension
* Updated DataStandardsWales-Appointment page to include DataStandardsWales-ClinicCode extension
* Removed search parameters from the Examples tab of the Immunization Profile page
* Added display column to FHIR Standards Wales Document Attribute guide page
* Added Value Set title to all Value Set guide pages
* Added SNOMED CT codes an expansion to DataStandardsWales-DocumentType guide page
* Corrected pagelink in Example-DataStandardsWales-DocumentReference-Provenance page
* Updated Example-DataStandardsWales-ServiceRequest-RadiologyOrder page to correct links
* Updated Allergy example pages to align naming between example files and example pages on the Implementation Guide and to correct the rendering of links
* Updated page.md pagelinks to shortened pagelinks throughout implementation guide

### v2.3.0 STU2
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
+ Added namespaces for WCRS DocumentId and WCRS DocumentSupersessionSetId values in Naming Systems table

### v2.2.0 STU2
Package: 
* {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions,text:Profiles and Extensions}}:
    * New Profiles
        * DataStandardsWales-Appointment        
    * Changes to Profiles
        * DataStandardsWales-Encounter
            * Updated version from 0.1.1 to 1.0.0
            * Updated status from draft to active
            * Added .extension:Speciality 
        * DataStandardsWales-Practitioner
            * Updated nadexIdentifier slice to include a fixed system url
        * DataStandardsWales-ServiceRequest
            * Updated version from 0.1.1 to 1.0.0
            * Updated status from draft to active
            * .code. Reverted minimum cardinality from 1..1 to 0..1 in line with UK Core
            * .performer. Added Must Support flag
        * DataStandardsWales-Observation-VitalSigns
            * Updated version from 1.0.0 to 1.1.0
            * Status fixed value removed
        * DataStandardsWales-Observation-VitalSigns-BMI
            * Updated version from 1.0.0 to 1.1.0
            * Status fixed value removed
        * DataStandardsWales-Observation-VitalSigns-BodyHeight
            * Updated version from 1.0.0 to 1.1.0
            * Status fixed value removed
        * DataStandardsWales-Observation-VitalSigns-BodyWeight
            * Updated version from 1.0.0 to 1.1.0
            * Status fixed value removed
    * New Extensions
        * DataStandardsWales-Speciality 
* {{pagelink:Home/FHIR-Assets/Naming-Systems.page.md,text:Naming Systems}}
    * New Naming Systems
        * Namespaces for PAS Appointment ids
        * Namespaces for PAS Sub-speciality codes
* {{pagelink:Home/Example-Index.page.md,text:Examples}}:
    * New Examples
        * Observation Vital Signs 
            * {{pagelink:Example-DataStandardsWales-Observation-VitalSigns-BMI,text: BMI}}
            * {{pagelink:Example-DataStandardsWales-Observation-VitalSigns-HeadCircumference,text: Head Circumference}}
            * {{pagelink:Example-DataStandardsWales-Observation-VitalSigns-MaternalHeight,text: Maternal Height}}
            * {{pagelink:Example-DataStandardsWales-Observation-VitalSigns-Weight,text: Weight}}
        * Provenance
            * {{pagelink:Example-DataStandardsWales-Provenance-DemographicUpdate, text:Example Provenance record linked to a Patient demographic update as result of an HL7v2 patient demographic update }}
            * {{pagelink:Example-DataStandardsWales-Provenance-MultipleTargets, text:Example Provenance record with multiple targets e.g. for growth chart observations}}
            * {{pagelink:Example-DataStandardsWales-Provenance-DemographicsAsRecorded, text:Example Provenance record showing the DemographicsAsRecorded extension}}
        * Questionnaire
            * {{pagelink:Example-DataStandardsWales-Questionnaire-GrowthChartCondition,text: Growth Chart Condition}}
        * Questionnaire Response
            * {{pagelink:Example-DataStandardsWales-QuestionnaireResponse-GrowthChartCondition,text: Growth Chart Condition Response}}
    * Removed Examples
        * Provenance
            * Example Provenance - Amend Device and Document Reference
            * Example Provenance - Amend where Device is unavailable
            * Example Provenance - Growth Charts 
Guide: 
* Added a new page to outline the DataStandardsWales-Appointment profile
* Updates to the DataStandardsWales-Provenance profile page, along with updated examples
* Added a new page to outline the DataStandardsWales-Speciality extension
* Updated relevant pages within the Guide to reflect changes outlined in Package
* Created a new section for {{pagelink:Home/Guidance/Growth-Charts,text: Growth Charts}} guidance

### v2.1.0 STU2
Package:
* {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions,text:Profiles and Extensions}}:
    * New Profiles
        * DataStandardsWales-Observation-VitalSigns
        * DataStandardsWales-Observation-VitalSigns-BMI
        * DataStandardsWales-Observation-VitalSigns-BodyWeight
        * DataStandardsWales-Observation-VitalSigns-BodyHeight
        * DataStandardsWales-Questionnaire
        * DataStandardsWales-QuestionnaireResponse
        * DataStandardsWales-RelatedPerson
    * Changes to Profiles
        * DataStandardsWales-AllergyIntolerance
            * Updated version from 0.1.0 to 0.1.1
            * .recorder. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
            * .asserter. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
            * .note.author. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
            * .reaction.note.author. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
        * DataStandardsWales-AllergyList
            * Updated version from 1.2.0 to 1.2.1
            * .note.author. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
        * DataStandardsWales-Device
            * Updated version from 0.0.1 to 0.0.2
            * note.author
                * Removed reference to HL7 Practitioner. Added reference to DataStandardsWales-Practitioner
                * Removed reference to HL7 Patient. Added reference to DataStandardsWales-Patient
                * Removed reference to HL7 RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
                * Removed reference to HL7 Organization. Added reference to DataStandardsWales-Organization
        * DataStandardsWales-DiagnosticReport
            * Updated version from 0.1.0 to 0.1.1
            * .basedOn. Removed reference to UKCore-ServiceRequest. Added reference to DataStandardsWales-ServiceRequest
        * DataStandardsWales-Encounter
            * Updated version from 0.1.0 to 0.1.1
            * .basedOn. Removed reference to HL7 ServiceRequest. Added reference to DataStandardsWales-ServiceRequest
            * .participant.individual. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
        * DataStandardsWales-Immunization
            * Updated version from 0.1.0 to 0.1.1
            * .note.author. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
        * DataStandardsWales-ImagingStudy
            * Updated version from 0.0.5 to 0.0.6
            * note.author
                * Removed reference to HL7 Practitioner. Added reference to DataStandardsWales-Practitioner
                * Removed reference to HL7 Patient. Added reference to DataStandardsWales-Patient
                * Removed reference to HL7 RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
                * Removed reference to HL7 Organization. Added reference to DataStandardsWales-Organization
        * DataStandardsWales-MedicationAdministration
            * Updated version from 1.1.0 to 1.1.1
            * .note.author. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
            * .performer.actor. 
                * Removed reference to UKCore-Device. Added reference to DataStandardsWales-Device
                * Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
        * DataStandardsWales-MedicationDispense
            * Updated version from 1.1.0 to 1.1.1
            * .performer.actor. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
            * .note.author. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson 
        * DataStandardsWales-MedicationList
            * Updated version from 1.1.0 to 1.1.1
            * .note.author. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson 
        * DataStandardsWales-MedicationRequest
            * Updated version from 1.1.0 to 1.1.1
            * .reported. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
            * .encounter. Removed reference to HL7 Encounter. Added reference to DataStandardsWales-Encounter
            * .requester. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
            * .performer. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
        * DataStandardsWales-MedicationStatement
            * Updated version from 1.1.0 to 1.1.1
            * .informationSource. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
            * note.author. 
                * Removed reference to HL7 RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
                * Removed reference to HL7 Practitioner. Added reference to DataStandardsWales-Practitioner
                * Removed reference to HL7 Patient. Added reference to DataStandardsWales-Patient
                * Removed reference to HL7 Organization. Added reference to DataStandardsWales-Organization
        * DataStandardsWales-Patient
            * Updated version from 1.2.0 to 1.2.1
            * .link.other
                * Removed reference to HL7 Patient. Added reference to DataStandardsWales-Patient
                * Removed reference to HL7 RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
        *  DataStandardsWales-Observation-Lab
            * Updated version from 0.1.0 to 0.1.1
            * .performer
                * Removed reference to HL7 Practitioner. Added reference to DataStandardsWales-Practitioner
                * Removed reference to HL7 Patient. Added reference to DataStandardsWales-Patient
                * Removed reference to HL7 Organization. Added reference to DataStandardsWales-Organization
                * Removed reference to HL7 RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
                * Removed reference to HL7 PractitionerRole. Added reference to DataStandardsWales-PractitionerRole
            * .note.author. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
        * DataStandardsWales-Observation
            * Updated version from 0.1.0 to 0.1.1
            * .performer. Removed reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
            * .note.author. Removed  reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
        * DataStandardsWales-Organization
            * Updated version from 1.1.0 to 1.1.1
            * .endpoint. Removed reference to HL7 Endpoint. Added reference to DataStandardsWales-Endpoint
        * DataStandardsWales-Practitioner
            * Updated version from 1.1.1 to 1.1.2
            * Added slice named NADEX-Identifier
        * DataStandardsWales-Provenance
            * Updated version from 0.0.1 to 0.0.2
            * .agent.who. Removed reference to HL7 RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
            * .agent.
                * Removed reference to HL7 Practitioner. Added reference to DataStandardsWales-Practitioner
                * Removed reference to HL7 PractitionerRole. Added reference to DataStandardsWales-PractitionerRole
                * Removed reference to HL7 RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
                * Removed reference to HL7 Patient. Added reference to DataStandardsWales-Patient
                * Removed reference to HL7 Device. Added reference to DataStandardsWales-Device
                * Removed reference to HL7 Organization. Added reference to DataStandardsWales-Organization
            * agent.onBehalfOf
                * Removed reference to HL7 Practitioner. Added reference to DataStandardsWales-Practitioner
                * Removed reference to HL7 PractitionerRole. Added reference to DataStandardsWales-PractitionerRole
                * Removed reference to HL7 RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
                * Removed reference to HL7 Patient. Added reference to DataStandardsWales-Patient
                * Removed reference to HL7 Device. Added reference to DataStandardsWales-Device
                * Removed reference to HL7 Organization. Added reference to DataStandardsWales-Organization
            * .signature.who.
                * Removed reference to HL7 Practitioner. Added reference to DataStandardsWales-Practitioner
                * Removed reference to HL7 PractitionerRole. Added reference to DataStandardsWales-PractitionerRole
                * Removed reference to HL7 RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
                * Removed reference to HL7 Patient. Added reference to DataStandardsWales-Patient
                * Removed reference to HL7 Device. Added reference to DataStandardsWales-Device
                * Removed reference to HL7 Organization. Added reference to DataStandardsWales-Organization
            * .signature.onBehalfOf.
                * Removed reference to HL7 Practitioner. Added reference to DataStandardsWales-Practitioner
                * Removed reference to HL7 PractitionerRole. Added reference to DataStandardsWales-PractitionerRole
                * Removed reference to HL7 RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
                * Removed reference to HL7 Patient. Added reference to DataStandardsWales-Patient
                * Removed reference to HL7 Device. Added reference to DataStandardsWales-Device
                * Removed reference to HL7 Organization. Added reference to DataStandardsWales-Organization
		* DataStandardsWales-ServiceRequest
            * Updated version from 0.1.0 to 0.1.1
            * .requester. Removed  reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
            * .performer. Removed  reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
            * .note.author. Removed  reference to UKCore-RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
        * DataStandardsWales-Specimen
            * Updated version from 0.1.0 to 0.1.1
            * .note.author
                * Removed reference to HL7 Practitioner. Added reference to DataStandardsWales-Practitioner
                * Removed reference to HL7 Patient. Added reference to DataStandardsWales-Patient
                * Removed reference to HL7 Organization. Added reference to DataStandardsWales-Organization
                * Removed reference to HL7 RelatedPerson. Added reference to DataStandardsWales-RelatedPerson
    * New Extensions
        * DataStandardsWales-RecordingSetting
* {{pagelink:Home/FHIR-Assets/Terminology,text:Terminology}}:
    * New Value Sets
        * DataStandardsWales-BloodPressure
        * DataStandardsWales-BloodPressureDiastolic
        * DataStandardsWales-BloodPressureSystolic
        * DataStandardsWales-BMI
        * DataStandardsWales-BodyHeightMeasurement
        * DataStandardsWales-BodyPosition
        * DataStandardsWales-BodyTemperature
        * DataStandardsWales-BodyWeightMeasurement
        * DataStandardsWales-HeadCircumferenceMeasurement
        * DataStandardsWales-HeartRate
        * DataStandardsWales-ObservationVitalSignsType
        * DataStandardsWales-OxygenSaturation
        * DataStandardsWales-QuestionnaireQuestionCodes
        * DataStandardsWales-RecordingSetting
        * DataStandardsWales-RespirationRate
    * New Code Systems
        * DataStandardsWales-RecordingSetting
* {{pagelink:Home/FHIR-Assets/Naming-Systems.page.md,text:Naming Systems}}
    * New Naming Systems
        * NADEX-Identifier
* {{pagelink:Home/Example-Index.page.md,text:Examples}}:
    * New Examples
        * Provenance
            * Example-DataStandardsWales-Provenance-Growth-Charts (Note: Example subsequently removed in v2.2.0 STU2)

Guide:
* Updated relevant pages within the Guide to reflect changes outlined in Package.
* General improvements including removing of duplicate sections, spelling mistakes and capitalisation of abbreviations (i.e. DM+D)
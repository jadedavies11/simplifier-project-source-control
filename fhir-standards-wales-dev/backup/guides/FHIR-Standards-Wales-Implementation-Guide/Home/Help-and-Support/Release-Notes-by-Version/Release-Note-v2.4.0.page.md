## {{page-title}}

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
### v2.5.0 STU2
The proposed removal of DataStandardsWales-Dosage, a profile of the Dosage DataType, has been postponed following feedback to further investigate potential impacts.

Package:
* Profiles and Extensions:
    * New Profiles
        * DataStandardsWales-MessageDefinition
        * DataStandardsWales-MessageHeader
    * New Message Definitions
        * MessageDefinition-DataStandardsWales-UEC-Arrival
        * MessageDefinition-DataStandardsWales-UEC-Discharge
        * MessageDefinition-DataStandardsWales-UEC-Triage
    * Changes to Profiles
        * DataStandardsWales-Appointment
            * Updated version from 1.1.0 to 1.2.0
            * .id and .title added
        * DataStandardsWales-Composition
            * Updated version from 0.1.0 to 0.2.0
            * .experimental. Updated from true to false
        * DataStandardsWales-Condition
            * Updated version from 0.0.1 to 0.1.0
            * .experimental. Updated from true to false
        * DataStandardsWales-Device
            * Updated version from 0.0.2 to 1.0.0
            * .status. Updated from draft to active
            * .experimental. Updated from true to false
            * Must Support flag added to .identifier:applicationInstanceId
        * DataStandardsWales-DiagnosticReport
            * Updated version from 0.1.3 to 0.2.0
            * .experimental. Updated from true to false
        * DataStandardsWales-DiagnosticReport-Lab
            * Updated version from 0.1.2 to 0.2.0
            * .experimental. Updated from true to false
        * DataStandardsWales-DocumentReference
            * Updated version from 0.0.1 to 0.1.0
            * .experimental. Updated from true to false
            * extension:versionR5 url changed to https://fhir.nhs.wales/StructureDefinition/Extension-DataStandardsWales-DocumentReference.version
            * extension:attesterR5 url changed to https://fhir.nhs.wales/StructureDefinition/Extension-DataStandardsWales-DocumentReference.attester
            * .content.attachment.language. Updated description and Requirements
            * .content.format. Updated description
            * .context.practiceSetting. Corrected ValueSet binding
            * .type. Increased minimum cardinality to 1
            * .category. Increased minimum cardinality to 1
        * DataStandardsWales-Encounter-UEC
            * Updated version from 0.0.2 to 0.1.0
            * .experimental. Updated from true to false
        * DataStandardsWales-Endpoint
            * Updated version from 0.0.5 to 1.0.0
            * .status. Updated from draft to active
            * .experimental. Updated from true to false
        * DataStandardsWales-ImagingStudy
            * Updated version from 0.1.0 to 0.2.0
            * .experimental. Updated from true to false
        * DataStandardsWales-Immunization
            * Updated version from 1.1.0 to 1.2.0
            * extension:DataStandardsWalesImmunizationBasedOn url changed to https://fhir.nhs.wales/StructureDefinition/Extension-DataStandardsWales-Immunization.basedOn
            * Amended Extension Elements names:
                * From Immunization.extension:DataStandardsWalesImmunizationBasedOn to Immunization.extension:immunizationBasedOnR5
                * From Immunization.extension:DataStandardsWalesAdministeredProduct to Immunization.extension:administeredProduct
                * From Immunization.extension:DataStandardsWalesForecastCreationSource to Immunization.extension:forecastCreationSource
                * From Immunization.extension:DataStandardsWalesDateProcedureLastUpdated to Immunization.extension:dateProcedureLastUpdated
        * DataStandardsWales-ImmunizationRecommendation
            * Updated version from 0.0.2 to 1.0.0
            * .status. Updated from draft to active
        * DataStandardsWales-MedicationRequest
            * Updated version from 1.2.0 to 1.3.0
            * .requestor. Cardinality changed from 1..1 to 0..1 to align with UKCore.
        * DataStandardsWales-Observation
            * Updated version from 0.1.3 to 1.0.0
            * .status. Updated from draft to active
            * .experimental. Updated from true to false
        * DataStandardsWales-Observation-Lab
            * Updated version from 0.1.2 to 0.2.0
            * .experimental. Updated from true to false
        * DataStandardsWales-Observation-VitalSigns
            * Updated version from 1.1.0 to 1.2.0
            * .status. Updated from draft to active
            * .description. Updated to reflect correct derivation
            * .subject. Removed references to HL7 Group, DataStandardsWales-Location and DataStandardsWales-Device
        * DataStandardsWales-Observation-VitalSigns-BMI
        	* Updated version from 1.1.1 to 1.2.0
            * .status. Updated from draft to active
            * .description. Updated to reflect correct derivation
        	* .code.coding. Valueset binding URL corrected
            * .subject. Removed differential to reflect the constraint in base profile
        * DataStandardsWales-Observation-VitalSigns-BodyHeight
        	* Updated version from 1.1.0 to 1.2.0
            * .status. Updated from draft to active
            * .description. Updated to reflect correct derivation
            * .code.coding:snomedCT. Removed description from the binding
            * .subject. Removed differential to reflect the constraint in base profile
        * DataStandardsWales-Observation-VitalSigns-BodyWeight
        	* Updated version from 1.1.0 to 1.2.0
            * .status. Updated from draft to active
            * .description. Updated to reflect correct derivation
            * .code.coding:snomedCT. Removed description from the binding
            * .subject. Removed differential to reflect the constraint in base profile
        * DataStandardsWales-Provenance
            * Updated version from 0.0.2 to 1.0.0
            * .status. Updated from draft to active
            * .experimental. Updated from true to false
        * DataStandardsWales-Questionnaire
        	* Updated version from 0.1.0 to 1.0.0
            * .status. Updated from draft to active
            * Added Must Support for .name, .title, .description and .purpose
         * DataStandardsWales-QuestionnaireResponse
        	* Updated version from 0.1.0 to 1.0.0
            * .status. Updated from draft to active
        * DataStandardsWales-ServiceRequest
        	* Updated version from 1.0.1 to 1.1.0
            * .experimental. Updated from true to false
	        * .reasonReference. Updated reference from UKCoreCondition to DataStandardsWalesCondition
        * DataStandardsWales-Specimen
            * Updated version from 0.1.1 to 0.2.0
            * .experimental. Updated from true to false
    * Changes to Message Definitions
        * DataStandardsWales-UEC-Arrival re-ordered metadata elements
        * DataStandardsWales-UEC-Discharge re-ordered metadata elements
        * DataStandardsWales-UEC-Triage re-ordered metadata elements
    * Changes to Extensions
        * Extension-DataStandardsWales-AdministeredProduct
            * Updated version from 0.1.0 to 1.0.0
            * .status. Updated from draft to active
        * Extension-DataStandardsWales-ClinicCode
            * Updated version from 0.0.1 to 1.0.0
            * .status. Updated from draft to active
        * Extension-DataStandardsWales-DateProcedureLastUpdated
            * Updated version from 0.1.0 to 1.0.0
            * .status. Updated from draft to active
        * Extension-DataStandardsWales-DemographicsAsRecorded
            * Updated version from 0.0.1 to 1.0.0
            * .status. Updated from draft to active
            * Added date.
        * Extension-DataStandardsWales-DocumentAttester
            * Updated version from 0.0.1 to 0.1.0
            * .experimental. Updated from true to false
            * Updated url and extension.url values to https://fhir.nhs.wales/StructureDefinition/Extension-DataStandardsWales-DocumentReference.attester
        * Extension-DataStandardsWales-DocumentAttribute
            * Updated version from 0.0.1 to 0.1.0
            * .experimental. Updated from true to false
            * Replaced Value Set in attributeName.value from FHIRStandardsWales-DocumentAttribute to DataStandardsWales-DocumentAttribute
        * Extension-DataStandardsWales-DocumentDigitalStatus
            * Updated version from 0.0.1 to 0.1.0
            * .experimental. Updated from true to false
            * Replaced value unknown with UNK in short description
        * Extension-DataStandardsWales-DocumentErrorAction
            * Updated version from 0.0.1 to 0.1.0
            * .experimental. Updated from true to false
            * Replaced Value Set in actionType.value from FHIRStandardsWales-DocumentErrorAction to DataStandardsWales-DocumentErrorAction
        * Extension-DataStandardsWales-DocumentErrorStatus
            * Updated version from 0.0.1 to 0.1.0
            * .experimental. Updated from true to false
            * Replaced Value Set in .value from FHIRStandardsWales-DocumentErrorStatus to DataStandardsWales-DocumentErrorStatus
        * Extension-DataStandardsWales-DocumentVersion
            * Updated version from 0.0.1 to 0.1.0
            * .experimental. Updated from true to false
            * Updated url and extension.url values to https://fhir.nhs.wales/StructureDefinition/Extension-DataStandardsWales-DocumentVersion
        * Extension-DataStandardsWales-ForecastCreationSource
            * Updated version from 0.1.0 to 1.0.0
            * .status. Updated from draft to active
        * Extension-DataStandardsWales-Immunization.basedOn
            * Updated version from 0.1.1 to 1.0.0
            * Updated url and extension.url values to https://fhir.nhs.wales/StructureDefinition/Extension-DataStandardsWales-Immunization.basedOn
            * .status. Updated from draft to active
        * Extension-DataStandardsWales-SingleRecord-AllergiesListConfirmedBy
            * Added version as 1.0.0
            * .status. Updated from draft to active
        * Extension-DataStandardsWales-SingleRecord-AllergiesListConfirmedDate
            * Updated version from 1.0.0 to 1.1.0
            * .status. Updated from draft to active
        * Extension-DataStandardsWales-SourceSystem
            * Updated version from 0.0.1 to 0.1.0
            * .experimental. Updated from true to false
        * Extension-DataStandardsWales-Speciality
            * Added version as 1.0.0
            * Added status to active
        * Extension-DataStandardsWales-UECDischargeInformationGiven
            * Updated version from 0.0.2 to 0.1.0
            * .experimental. Updated from true to false
* Terminology:
    * New Code Systems
        * DataStandardsWales-DocumentAttribute
        * DataStandardsWales-DocumentErrorAction
        * DataStandardsWales-DocumentErrorStatus
        * DataStandardsWales-UEC-MessageEvent
    * Removed Code Systems
        * DataStandardsWales-DocumentCategory
            * Removed and replaced with a SNOMED CT ValueSet
        * DataStandardsWales-WRRSTaskType
            * Initially introduced as an optional CodeSystem but not implemented. Removed to prevent inappropriate use
        * FHIRStandardsWales-DocumentAttribute
            * Replaced by value set DataStandardsWales-DocumentAttribute
        * FHIRStandardsWales-DocumentErrorAction
            * Replaced by value set DataStandardsWales-DocumentErrorAction
        * FHIRStandardsWales-DocumentErrorStatus
            * Replaced by value set DataStandardsWales-DocumentErrorStatus
    * Changes to Code Systems
        * DataStandardsWales-DocumentDigitalStatus
            * Updated version from 0.0.1 to 0.1.0
            * .experimental. Updated from true to false
            * Removed 'unknown' code
        * DataStandardsWales-PatientRecordType
            * Updated version from 0.0.1 to 1.0.0
            * .experimental. Updated from true to false
            * status. Updated from draft to active
        * MessageEvents
            * Updated version from 0.0.1 to 1.0.0
            * .experimental. Updated from true to false
            * .status. Updated from draft to active
        * WPASAdmitSource
            * Updated version from 0.0.1 to 1.0.0
            * .experimental. Updated from true to false
            * .status. Updated from draft to active
        * WPASEventType
            * Updated version from 0.0.1 to 1.0.0
            * .experimental. Updated from true to false
            * .status. Updated from draft to active
        * WPASReferralSource
            * Updated version from 0.0.1 to 1.0.0
            * .experimental. Updated from true to false
            * .status. Updated from draft to active
        * WPASSourceAdmission
            * Updated version from 0.0.1 to 1.0.0
            * .experimental. Updated from true to false
            * .status. Updated from draft to active
    * New Value Sets
        * DataStandardsWales-BloodPressure-AverageSystolic
        * DataStandardsWales-DocumentAttribute
        * DataStandardsWales-DocumentErrorAction
        * DataStandardsWales-DocumentErrorStatus
        * DataStandardsWales-MessageEvent
    * Removed Value Sets
        * DataStandardsWales-QuestionnaireQuestionCodes
            * Initially introduced as an optional ValueSet but not implemented. Removed to prevent inappropriate use
        * DataStandardsWales-WRRSTaskType
            * Initially introduced as an optional ValueSet but not implemented. Removed to prevent inappropriate use
        * FHIRStandardsWales-DocumentAttribute
            * Replaced by value set DataStandardsWales-DocumentAttribute
        * FHIRStandardsWales-DocumentErrorAction
            * Replaced by value set DataStandardsWales-DocumentErrorAction
        * FHIRStandardsWales-DocumentErrorStatus
            * Replaced by value set DataStandardsWales-DocumentErrorStatus
    * Changes to Value Sets
        * DataStandardsWales-BloodPressure
            * Updated version from 1.0.0 to 1.1.0
            * Rebased the content of the value set to UKCore-BloodPressure v1.0.0 which is not yet included in a balloted release
        * DataStandardsWales-DocumentCategory
            * Updated version from 0.0.1 to 0.1.0
            * .experimental. Updated from true to false
            * .compose.include.system. Removed deprecated CodeSystem-DataStandardsWales-DocumentCategory and replaced with WRTS ValueSet DataStandardsWales-DocumentCategory
        * DataStandardsWales-DocumentDigitalStatus
            * Updated version from 0.0.1 to 0.1.0
            * .experimental. Updated from true to false
            * Added v.3 NullFlavor Code System
            * Removed .definition
        * DataStandardsWales-DocumentType
            * Updated version from 0.0.2 to 0.1.0
            * .experimental. Updated from true to false
            * Added 'Record composition type' simple reference set to description.
        * DataStandardsWales-EncounterType
            * Updated version from 1.0.0 to 1.1.0
            * Updated SNOMED CT 20250409 version
            * Expanded SNOMED CT codes to show 50 concepts as sample
        * DataStandardsWales-Observation-VitalSigns
            * Updated version from 1.0.0 to 1.1.0
            * Corrected all canonical references to constituent value sets
            * Removed expansion codes, which can be found in the constituent value sets
        * DataStandardsWales-Occupation
            * Updated version from 0.0.5 to 1.0.0
            * .experimental. Updated from true to false
            * status. Updated from draft to active
            * Updated SNOMED CT 20250409 version
            * Expanded SNOMED CT codes to show 50 concepts as sample
        * DataStandardsWales-PatientRecordType
            * Updated version from 0.0.1 to 1.1.0
            * .experimental. Updated from true to false
            * status. Updated from draft to active
        * DataStandardsWales-ProvenanceActivity
            * Updated version from 0.0.1 to 1.0.0
            * .experimental. Updated from true to false
             * status. Updated from draft to active
		* DataStandardsWales-RecordingSetting
			* Updated version from 1.0.0 to 1.0.1
			* Valueset binding url corrected
        * DataStandardsWales-Religion 'contains' tags corrected
		* MessageEvents
            * Updated version from 0.0.1 to 1.0.0
            * .status. Updated from draft to active
            * .experimental. Updated from true to false
            * Renamed id from DataStandardsWales-DocumentCategory to MessageEvents
            * Renamed url from "https://fhir.nhs.wales/message-events" to "https://fhir.nhs.wales/ValueSet/message-events"
        * PASAdmitSource
			* Updated version from 0.0.1 to 1.0.0
            * .experimental. Updated from true to false
            * .status. Updated from draft to active
			* Valueset binding url corrected
        * PASEventType
           * Updated version from 0.0.1 to 1.0.0
           * .experimental. Updated from true to false
           * .status. Updated from draft to active
        * PASReferralSource
            * Updated version from 0.0.1 to 1.0.0
            * .experimental. Updated from true to false
            * .status. Updated from draft to active
        * PASSourceAdmission
            * Updated version from 0.0.1 to 1.0.0
            * .experimental. Updated from true to false
            * .status. Updated from draft to active
* Naming Systems:
    * Changes to Naming Systems
        * New Naming Systems
            * Namespaces for PAS link identifiers
        * Updated Naming Systems
            * Corrected Sub-Specialty id from Speciality to Specialty
            * Corrected element descriptors for DataStandardsWales-SBUHB-PAS-LinkIdentifier and DataStandardsWales-VUNHST-PAS-LinkIdentifier
* Examples:
    * New Examples
        * FHIR Messaging guidance
            * Example Message Bundle - Submit Clinician (Logical Referencing)
            * Example Message Bundle - Submit Clinician (Literal FHIR Referencing)
            * Example Message Definition - Submit Clinician
        * Urgent and Emergency Care
            * Example Message Bundle - UEC Arrival UHWEUMI (UHW Emergency Unit Minor Injuries)
            * Example Message Bundle - UEC Triage UHWEUMI (UHW Emergency Unit Minor Injuries)
            * Example Message Bundle - UEC Discharge UHWEUMI (UHW Emergency Unit Minor Injuries)
    * Changes to Examples
        * Allergy Degraded
            * Bundle-Degraded allergies
                * Updated full url
                * Updated url for extension:ethnicCategory from https://fhir.nhs.uk/StructureDefinition/Extension-UKCore-EthnicCategory to https://fhir.hl7.org.uk/StructureDefinition/Extension-UKCore-EthnicCategory
                * Changed code for extension:religion
        * Appointment
            * Renamed example from Example-DataStandardsWales-Appointment-GenSurgery-FollowUp to Example-DataStandardsWales-Appointment-GenSurgery
        * Document Reference
            * DocumentReference-EncounterBased
                * Changes to align with updates to the DocumentReference profile and associated value sets
                * Extension urls updated for R5 backports
            * DocumentReference-EventBased
                * Changes to align with updates to the DocumentReference profile and associated value sets
                * Extension urls updated for R5 backports
            * DocumentReference-NotEventBased changes made to align with updates to the DocumentReference profile and associated value sets
            * DocumentReference-MisfiledNotEventBased
                * Changes to align with updates to the DocumentReference profile and associated value sets
                * Changed id from Example-DataStandardsWales-DocumentReference-MisfiledNotEventBased to Example-DSW-DocumentReference-MisfiledNotEventBased
            * DocumentReference-Provenance
                * Changes to align with updates to the DocumentReference profile and associated value sets
                * Updated url for .content.attachment
        * Endpoint
            * Endpoint - Dicom Ima added HL7 namespace
        * Immunization
            * Immunization - Not Given added Z suffix to .occurrenceDateTime
        * Observation
            * Observation - ACVPU added HL7 namespace
            * Observation - Blood pressure added HL7 namespace
            * Observation - Body temperature added HL7 namespace
            * Observation - Respiratory rate added HL7 namespace
        * Observation Vital Signs
            * Observation Vital Signs - Head Circumference changed id from Example-DataStandardsWales-Observation-VitalSigns-HeadCircumference to Example-DSW-Observation-VitalSigns-HeadCircumference
        * Observation Vital Signs BMI
            * Observation Vital Signs BMI added HL7 namespace
        * Observation Vital Signs Body Height
            * Observation Vital Signs - Maternal Height added HL7 namespace
        * Observation Vital Signs Weight
            * Observation Vital Signs - Weight added HL7 namespace
        * Patient
            * Patient - Alice Jones
                * Changed code structure for extension:birthSex
                * Updated url for extension:ethnicCategory from https://fhir.nhs.uk/StructureDefinition/Extension-UKCore-EthnicCategory to https://fhir.hl7.org.uk/StructureDefinition/Extension-UKCore-EthnicCategory
                * Changed code for extension:religion
            * Patient - Harold James
                * Updated url for extension:ethnicCategory from https://fhir.nhs.uk/StructureDefinition/Extension-UKCore-EthnicCategory to https://fhir.hl7.org.uk/StructureDefinition/Extension-UKCore-EthnicCategory
        * Provenance
            * Provenance - Demographics as recorded within care document changed id from Example-DataStandardsWales-Provenance-DocumentReferenceDemographics to  Example-DSW-Provenance-DocumentReferenceDemographics
        * Questionnaire Response
            * Questionnaire Response - Growth Chart Condition
                * Changed id from Example-DataStandardsWales-QuestionnaireResponse-GrowthChartCondition to Example-DSW-QuestionnaireResponse-GrowthChartCondition
                * Added HL7 namespace
        * Related Person
            * Related Person - Natural Mother added HL7 namespace
    * Removed Examples
        * DataStandardsWales-Encounter-Outpatient

Guide:
* General improvements to IG that include fixing spelling mistakes, correcting grammatical errors and formatting, and correcting hyperlinks.
* Alphabetised yaml toc files
* Standardised examples names in Example Index page
* Standardised resource links in IG pages
* Added Index to Growth Charts yaml toc file
* Added Data Exchange category to Resource Index
* Added ValueSets DataStandardsWales-EncounterType & PASEventType to yaml toc file
* Added a new page to outline the DataStandardsWales-MessageDefinition profile
* Added a new page to outline the DataStandardsWales-MessageHeader profile
* Added new pages to outline the Message Definitions created in this release
* Added new pages to outline the Code Systems created in this release
* Added new pages to outline the Value Sets created in this release
* Added new pages to outline the Examples created in this release
* Added FHIR Messaging Guidance page
* Added Urgent and Emergency Care Guidance page
* Added information to the Care Documents Guidance page
* Added Mandatory and Must Support Data Elements section to DataStandardsWales-Device page
* Added Provenance Extensions section to Provenance Guidance page
* Added WRTS contact details to DataStandardsWales-EncounterType Value Set guide page
* Added WRTS contact details to DataStandardsWales-DocumentCategory Value Set guide page
* Added WRTS contact details to DataStandardsWales-Occupation Value Set guide page
* Added WRTS contact details to DataStandardsWales-Religion Value Set guide page
* Corrected title page for Extension Data Standards Wales Speciality to align with IG standards
* Corrected pagelinks for Example Encounter - In-Progress Emergency Admission in Example Index page
* Moved DataStandardsWales-Endpoint from Diagnostics to Entities in the Resource Index
* Removed most page warnings, restricting them to home page, main index pages and specific content that is under development
* Removed duplicated examples from DataStandardsWales-Observation guide page. All examples are now located in the Examples tab of the Profile Content table
* Removed DataStandardsWales-QuestionnaireQuestionCodes documentation
* Removed DataStandardsWales-WRRSTaskType Code System and Value Set documentation
* Renamed Naming Systems page in Design tab to Naming Systems Design
* Renamed Code System and Value Set pages from FHIRStandardsWales-DocumentAttribute to DataStandardsWales-DocumentAttribute
* Renamed Code System and Value Set pages from FHIRStandardsWales-DocumentErrorAction to DataStandardsWales-DocumentErrorAction
* Renamed Code System and Value Set pages from FHIRStandardsWales-DocumentErrorStatus to DataStandardsWales-DocumentErrorStatus
* Renamed Example-DataStandardsWales-Bundle-Allergies-Update page to Example-DataStandardsWales-Bundle-Allergies-Upgrade
* Replaced HL7 R5 AuditEvent link with HL7 R4 AuditEvent link in DataStandardsWales-AuditEvent IG page
* Replaced unknown with UNK in DataStandardsWales-DocumentReference IG page
* Updated Draft/Active status and removed Experimental flag on the Home page to mirror changes to the profiles
* Updated left sided navigation panes and asset indexes for easier discovery
* Updated wording on DataStandardsWales-Observation-VitalSigns Profile pages to clarify derivation.
* Updated narrative content to reflect revised understanding of experimental as exploratory e.g. for prototyping
* Updated Purpose narrative for DataStandardsWales-DocumentAttester and DataStandardsWales-DocumentVersion pages
* Updated DataStandardsWales-DocumentReference page to reflect cardinality changes
* Updated page link in FHIR Assets Naming System from Naming System to Naming Systems Design
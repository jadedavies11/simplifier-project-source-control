## {{page-title}}

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
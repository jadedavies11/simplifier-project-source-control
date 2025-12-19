## {{page-title}}

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
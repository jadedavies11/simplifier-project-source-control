## {{page-title}}

As part of our commitment to quality assurance and interoperability, we undertook an exercise to review and align the existing FHIR Standards Wales Package with UK Core STU2 (fhir.r4.ukcore.stu2 2.0.1). This resulted in us rationalising the FHIR Standards Wales Package where possible, removing detail that can already be derived from UK Core STU2, whilst still adhering to the principles of FHIR and supporting Wales specific content where required. 
In addition to the removal of replicate content, the following changes were made: 

Package:
* {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions,text:Profiles and Extensions}}:
    * Changes to Profiles
        * DataStandardsWales-AllergyIntolerance
            * Updated version number from 1.0.0 to 1.1.0
            * Reference changes:
                * .encounter. Removed reference to UKCore-Encounter. Added reference to DataStandardsWales-Encounter
                * extension:evidence. Removed reference to UKCore-DiagnosticReport. Added reference to DataStandardsWales-DiagnosticReport
            * Binding strength changes:
                * .reaction.substance. From extensible to preferred
	            * .reaction.manifestation. From extensible to preferred
	            * .reaction.exposureRoute. From extensible to preferred
        * DataStandardsWales-AllergyList
            * Updated version number from 1.1.0 to 1.2.0
            * Reference changes:
                * .encounter. Removed reference to UKCore-Encounter. Added reference to DataStandardsWales-Encounter
                * .source. Removed reference to Device. Added reference to DataStandardsWales-Device
        * DataStandardsWales-DiagnosticReport
            * Updated version number from 0.0.5 to 0.1.0
            * Reference changes:
                * .performer. Added reference to CareTeam
            * Removed Slices:
                * .code
                * .conclusionCode
        * DataStandardsWales-DiagnosticReport-Lab
            * Updated version number from 0.0.5 to 0.1.0
            * .conclusionCode.Removed Slice
            * Reference changes:
                *  .basedOn. Removed reference to HL7 ServiceRequest. Added reference to UKCore-ServiceRequest
        * DataStandardsWales-Dosage   
            * Updated version number from 0.0.5 to 0.1.0
            * All Must Support flags removed 
            * Binding strength changes:
                * .asNeeded[]. From example to preferred
            * Binding terminology changes:
                * .site. Removed binding to value set SNOMEDCTAnatomicalStructureForAdministrationSiteCodes. Added binding to value set UKCoreBodySite. Binding strength set as preferred
                * .route. Removed binding to value set SNOMEDCTAdministrationMethodCodes. Added binding to value set UKCoreSubstanceOrProductAdministrationRoute. Binding strength set as preferred
                * .method. Removed binding to value set SNOMEDCTAdministrationMethodCodes. Added binding to value set UKCoreUKCoreMedicationDosageMethod. Binding strength set as preferred 
         * DataStandardsWales-Encounter
            * Updated version number from 0.0.5 to 0.1.0
            * Must Support changes:
                * .reasonCode. Added must support
	            * .reasonReference. Added must support
	        * Extension changes:
	            * .hospitalization. Added .extension:admissionMethod 
            * Reference changes:
                * .reasonReference. Removed reference to UKCore-Observation. Added reference to DataStandardsWales-Observation.
                * .reasonReference. Removed reference to HL7 Condition. Added reference to UKCore-Condition.
                *.reasonReference. Removed reference to HL7 Procedure. Added reference to UKCore-Procedure.
        * DataStandardsWales-ImagingStudy
            * Reference changes:
                * .reasonReference. Removed HL7 Condition. Added reference to UKCore-Condition
        * DataStandardsWales-Immunization
            * Updated version number from 0.0.5 to 0.1.0
            * Binding strength changes:
	            *.statusReason. From example to preferred
	        * Binding terminology changes:
	            * .vaccineCode. Added binding to value set UKCore-VaccineCode. Binding strength set as preferred
	            * .site. Removed binding to value set UKCore-BodySite. Added binding to value set UKCore-ImmunizationAdministrationBodySite. Binding strength set as preferred
	            * .route. Added binding to value set UKCore-SubstanceOrProductAdministrationRoute. Binding strength set as preferred
            * Reference changes:
                * .protocolApplied.authority . Removed reference to UKCore-Organization. Added reference to DataStandardsWales-Organization
        * DataStandardsWales-Location
            * Updated version number from 1.0.1 to 1.1.0
        * DataStandardsWales-Medication
            * Updated version number from 1.0.0 to 1.1.0
            * Reference changes:
                * .manufacturer. Added reference to DataStandardsWales-Organization
                * .ingredient.item[]. Removed reference to Medication. Added reference to DataStandardsWales-Medication
        * DataStandardsWales-MedicationAdministration
            * Updated version number from 1.0.1 to 1.1.0
            * Reference changes:
                * .reasonReference. Removed references to UKCore-Observation and UKCore-DiagnosticReport. Added references to DataStandardsWales-Observation and DataStandardsWales-DiagnosticReport
                * .performer.actor. Removed reference to UKCore-Device. Added reference to DataStandardsWales-Device
            * Binding strength changes:
                * .dosage.site. From extensible to preferred
                * .dosage.route. From extensible to preferred
                * .dosage.method. From extensible to preferred
        * DataStandardsWales-MedicationDispense
            * Updated version number from 1.0.1 to 1.1.0
            * Must Support changes:
                * .dosageInstruction.text. Added must support
                * .dosageInstruction.timing. Added must support
                * .dosageInstruction.doseAndRate. Added must support
                * .dosageInstruction.doseAndRate.dose[]. Added must support
                * .dosageInstruction.doseAndRate.rate[]. Added must support
            * Binding strength changes:
                * .dosageInstruction.site. From extensible to preferred
                * .dosageInstruction.route. From extensible to preferred
                * .dosageInstruction.method. From extensible to preferred
            * Binding terminology changes:
                * .dosageInstruction.asNeeded[]. Removed binding to value set UKCoreMedicationPrecondition. Added binding to value set SNOMEDCTMedicationAsNeededReasonCodes. Binding strength set as preferred     
            * Reference changes:
                * .context. Removed reference to UKCore-Encounter. Added reference for DataStandardsWales-Encounter
                * .performer.actor. Removed reference to UKCore-Device. Added reference for DataStandardsWales-Device
            * Cardinality change:
                * .receiver. Cardinality changed from 0:1 to 0:* by UK Core STU2
        * DataStandardsWales-MedicationList
            * Updated version number from 1.0.0 to 1.1.0
            * .source. Removed reference to UKCore-Device.Added reference for DataStandardsWales-Device
        * DataStandardsWales-MedicationRequest 
            * Updated version number from 1.0.0 to 1.1.0  
            * Must Support changes:
                * .dosageInstruction. Added must support
                * .dosageInstruction.text. Added must support
                * .dosageInstruction.timing. Added must support
                * .dosageInstruction.doseAndRate. Added must support
                * .dosageInstruction.doseAndRate.dose[]. Added must support
                * .dosageInstruction.doseAndRate.rate[]. Added must support
            * Binding strength changes:
                * .dosageInstruction.site. From extensible to preferred
                * .dosageInstruction.route. From extensible to preferred
                * .dosageInstruction.method. From extensible to preferred
            * Binding terminology changes:
                * .dosageInstruction.asNeeded[]. Removed binding to value set UKCoreMedicationPrecondition. Added binding to value set SNOMEDCTMedicationAsNeededReasonCodes. Binding strength set as preferred     
            * Reference changes:
                * .requester. Removed reference to Device. Added reference to DataStandardsWales-Device
                * .reasonReference. Removed Reference to UK Core Observation. Added Reference to DataStandardsWales-Observation
        * DataStandardsWales-MedicationStatement
            * Updated version number from 1.0.0 to 1.1.0
            * Must Support changes:
                * .dosage. Added must support
            * Binding strength changes:
                * .dosage.site. From extensible to preferred
                * .dosage.route. From extensible to preferred
                * .dosage.method. From extensible to preferred
            * Binding terminology changes:
                * .dosage.asNeeded[]. Removed binding to value set UKCoreMedicationPrecondition. Added binding to value set SNOMEDCTMedicationAsNeededReasonCodesSet. Binding strength set as preferred
            * Reference changes:
                * .basedOn. Removed reference to UKCore-ServiceRequest. Added reference to DataStandardsWales-ServiceRequest
                * .reasonReference. Removed reference to HL7 Condition. Added reference to UKCore-Condition
        * DataStandardsWales-Observation
            * Updated version number from 0.0.6 to 0.1.0
            * Reference changes:
                * .basedOn. Removed reference to MedicationRequest. Added reference to DataStandardsWales-MedicationRequest
                * .partOf. Removed references to MedicationAdministration, MedicationDispense, MedicationStatement, Procedure and Immunization. Added references to DataStandardsWales-MedicationAdministration, DataStandardsWales-MedicationDispense, DataStandardsWales-MedicationStatement, DataStandardsWales-Immunization, and UKCore-Procedure
                * .subject. Removed reference to Device. Added reference to DataStandardsWales-Device
                * .note.author[]. Added references to UKCore-RelatedPerson, DataStandardsWales-Organization, DataStandardsWales-Patient, and DataStandardsWales-Practitioner
                * .device. Removed reference to Device. Added reference to DataStandardsWales-Device
                * .hasMember. Added references to QuestionnaireResponse and MolecularSequence
            * Slices removed:
                * .code.coding
                * .coding:snomedCT
                * .coding:loinc
                * .bodySite.coding
                * .bodySite.coding:snomedCT
        * DataStandardsWales-Observation-Lab
            * Updated version from 0.0.5 to 0.1.0
            * Reference changes:
                * .subject. Removed references to Group, Device and DataStandardWales-Location
                * .device. Removed reference to Device. Added reference to DataStandardWales-Device
                * .hasMember. Added references to QuestionnaireResponse and MolecularSequence
            * Binding terminology changes:
                * .code. Removed binding to value set LOINCCodes. Added binding to value set UKCore-PathologyAndLaboratoryMedicineObservables. Binding strength set as preferred
            * Slices removed:
                * .code.coding
                * .code.coding:snomedCT
                * .code.coding:loinc
                * .bodySite.coding
                * .bodySite.coding:snomedCT
                * .component.code.coding 
                * .component.code.coding:snomedCT
        * DataStandardsWales-Organization
            * Updated version from 1.0.0 to 1.1.0
        * DataStandardsWales-Patient
            * Updated version from 1.1.0 to 1.2.0
            * Slicing changes:
                * .identifier:bcuhbCentralPasIdentifier renamed to  .identifier:bcuhbPasIdentifier. Fixed Value, Short Description and Definition updated to correspond.
            * Slices removed:
                * .identifier. Removed slices for bcuhbEastPasIdentifier and bcuhbWestPasIdentifier
        * DataStandardsWales-Practitioner
            * Updated version number from 1.0.1 to 1.1.1 
            * Must Support changes:
                * .identifier.system. Added must support
                * .identifier.value. Added must support
                * .identifier:gdcNumber.system. Added must support
                * .identifier:gdcNumber.value. Added must support
                * .identifier:gmcNumber.system. Added must support
                * .identifier:gmcNumber.value. Added must support
                * .identifier:gmpNumber.system. Added must support
                * .identifier:gmpNumber.value. Added must support
                * .identifier:hcpcNumber.system. Added must support
                * .identifier:hcpcNumber.value. Added must support
                * .identifier:nmcNumber.system. Added must support
                * .identifier:nmcNumber.value. Added must support
                * .identifier:gphcCode.system. Added must support
                * .identifier:gphcCode.value. Added must support
                * .identifier:sdsUserId.system. Added must support
                * .identifier:sdsUserId.value. Added must support
                * .name.family. Added must support
                * .telecom. Added must support
                * .telecom.system. Added must support
                * .telecom.value. Added must support
        * DataStandardsWales-PractitionerRole
            * Updated version from 1.0.0 to 1.1.0
            * Must Support changes:
                * .location. Added must support
                * .telecom.system. Added must support
                * .telecom.value. Added must support
        * DataStandardsWales-ServiceRequest
            * Updated version number from 0.0.5 to 0.1.0
            * Reference changes:
                * .note.author[]. Removed references to Organization, Patient, Practitioner, and RelatedPerson. Added references to DataStandardsWales-Organization, DataStandardsWales-Patient, DataStandardsWales-Practitioner, and UKCore-RelatedPerson
                * .relevantHistory. Removed reference to Provenance. Added reference to DataStandardsWales-Provenance
            * Binding terminology changes:
                * .orderDetail. Removed ValueSet ServiceRequestOrderDetailsCodes. Replaced with ValueSet UKCoreProcedureCode. Binding changed to preferred
        * DataStandardsWales-Specimen
            * Updated version from 0.0.5 to 0.1.0
            * Binding terminology changes:
                * .type. Removed binding to value set v2.0487. Added binding to value set https://fhir.hl7.org.uk/ValueSet/UKCore-SpecimenType
                * .condition. Removed binding to value set v2.0493. Added binding to value set UKCore-BiopsyState
            * Slices removed:
                * .type.coding
                * .type.coding:snomedCT
                * .collection.bodySite.coding 
                * .collection.bodySite.coding:snomedCT
            * Reference changes:
                * .subject. Removed reference to Device. Added reference to DataStandardsWales-Device
            * Extension changes:
                * Added extension for sampleCategory
                * .collection. Added extension for specialHandling 
                * .collection.collector. Added extension for collectionCollectorR5
                * .collection.bodySite. Added extension for bodySiteReference

Examples:
* Removed Dosage Examples
* Fixed render issues in Immunizations:
    * {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/Examples/Immunization/Example-DataStandardsWales-Immunization-FluVaccine.page.md,text:Flu Vaccine}}  
    * {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/Examples/Immunization/Example-DataStandardsWales-Immunization-NotGiven.page.md,text:Not Given}}    
    * {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/Examples/Immunization/Example-DataStandardsWales-Immunization-ParentPresent.page.md,text:Parent Present}}  
        
Guide:
* Created a new section for {{pagelink:Home/Guidance/provenance}} guidance
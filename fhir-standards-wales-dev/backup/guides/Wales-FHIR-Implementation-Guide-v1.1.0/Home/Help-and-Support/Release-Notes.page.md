## {{page-title}}

This page describes the published versions of this implementation guide and differences between versions:

### v2.0.0 STU2
Package:
* {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions,text:Profiles and Extensions}}:
    * Changes to Profiles
        * DataStandardsWales-AllergyList
            * Aligned with UKCore STU2
        * DataStandardsWales-DiagnosticReport
            * Aligned with UKCore STU2
        * DataStandardsWales-DiagnosticReport-Lab
            * Aligned with UKCore STU2
        * DataStandardsWales-Location
            * Aligned with UKCore STU2
        * DataStandardsWales-Medication
            * Aligned with UKCore STU2
            * Updated references
        * DataStandardsWales-MedicationAdministration
            * Aligned with UKCore STU2
            * Updated References
        * DataStandardsWales-Observation
            * Aligned with UKCore STU2
            * References to UKCore and DataStandardsWales profiles updated
        * DataStandardsWales-Immunization
            * Updated version from 0.0.5 to 0.1.0
            * Profile changed from experimental to draft
            * ValueSet UKCore-ReasonImmunizationNotAdministered binding changed to Preferred in Immunization.statusReason
            * ValueSet updated for Immunization.site from UKCore-BodySite to UKCore-ImmunizationAdministrationBodySite and binding is Preferred
            * ValueSet for Immunization.protocolApplied.targetDisease remained as ValueSet covid-19-diseases
        * DataStandardsWales-Practitioner
            * Updated version from 1.0.1 to 1.1.1
        * DataStandardsWales-Observation-Lab
            * Updated version from 0.0.5 to 0.1.0
            * ValueSet updated for Observation.code from observation-codes to UKCore-PathologyAndLaboratoryMedicineObservables
            * Removed Slices
                * Observation.code.coding
                * Observation.code.coding:snomedCT
                * Observation.code.coding:loinc
                * Observation.bodySite.coding
                * Observation.bodySite.coding:snomedCT
                * Observation.component.code.coding
                * Observation.component.code.coding:snomedCT
            * Removed HL7 Group, HL7 Device & DataStandardsWales-Location from Observation.subject
            * Replace HL7 Device with DataStandardsWales-Device in Observation.specimen
            * Added HL7 QuestionnaireResponse & HL7 MolecularSequence to Observation.hasMember
        * DataStandardsWales-Organization
            * Updated version from 1.0.0 to 1.1.0
        * DataStandardsWales-Dosage
            * Updated version from 0.0.5 to 0.1.0 
        * DataStandardsWales-Encounter
            * Updated version from 0.0.5 to 0.1.0
            * Extension removed:
                * Encounter.hospitalization.extension:admissionMethod
            * Added Extension:
                * Encounter.hospitalization.extension:admissionMethod
        * DataStandardsWales-AllergyIntolerance
            * Updated version from 1.0.0 to 1.1.0
            * AllergyIntolerance.encounter updated with DataStandardsWales-Encounter resource
            * ValueSet Binding changed to Preferred:
                * UKCore-AllergySubstance in AllergyIntolerance.reaction.substance
                * UKCore-AllergyManifestation in AllergyIntolerance.reaction.manifestation
                * UKCore-SubstanceOrProductAdministrationRoute in AllergyIntolerance.reaction.exposureRoute
        * DataStandardsWales-Patient
            * Updated version from 1.1.0 to 1.2.0
            * Slice renamed to bcuhbPasIdentifier
            * Fixed value in System updated to https://fhir.bcuhb.nhs.wales/Id/pas-identifier
            * Removed Slices: 
                * Patient.identifier:bcuhbEastPasIdentifier
                * Patient.identifier:bcuhbWestPasIdentifier          
        * DataStandardsWales-MedicationList
            * Updated version from 1.0.0 to 1.1.0  
        * DataStandardsWales-MedicationRequest
            * Updated version from 1.0.0 to 1.1.0
            * MedicationRequest.requester updated with DataStandardsWales-Device resource replacing HL7 Device
            * MedicationRequest.reasonReference updated with DataStandardsWales-Observation resource replacing UK Core Observation 
        * DataStandardsWales-PractitionerRole
            * Updated version from 1.0.0 to 1.1.0
        * DataStandardsWales-Specimen
            * Updated version from 0.0.5 to 0.1.0
            * New Extension-UKCore-SampleCategory added in Specimen.extension:sampleCategory
            * For Specimen.type:
                * Slice removed
                * New ValueSet UKCore-SpecimenType added and binding is Preferred
            * Replaced HL7 Device with DataStandardsWales-Device in Specimen.subject
            * New extension added http://hl7.org/fhir/StructureDefinition/specimen-specialHandling in Specimen.collection.extension:specialHandling
            * New extension-Specimen.collection.collector added in Specimen.collection.collector.extension:collectionCollectorR5
            * For Specimen.collection.bodySite.extension:bodySiteReference:
                * Slice removed
                * New Extension-UKCore-BodySiteReference added
            * ValueSet v2.0493 replaced with ValueSet UKCore-BiopsyState in Specimen.condition
                
### v1.2.0 STU1
Package:
* {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions,text:Extensions}}:
    * Changes to Profiles    
        * DataStandardsWales-AllergiesList
            * Added Extensions for:
                * DataStandardsWales-SingleRecord-AllergiesListUpdated
                * DataStandardsWales-SingleRecord-AllergiesListConfirmedDateurceTimestamp
                * DataStandardsWales-SingleRecord-AllergiesListConfirmedBy
    * New Extensions
        * DataStandardsWales-SingleRecord-AllergiesListUpdated
        * DataStandardsWales-SingleRecord-AllergiesListConfirmedDateurceTimestamp
        * DataStandardsWales-SingleRecord-AllergiesListConfirmedBy
    * Changes to Extensions
        * DataStandardsWales-CDRPatientRecordType
            * Removed this extension as the data item will be captured in tags
        * DataStandardsWales-CDRSourceTimestamp
            * Removed this extension as the data item will be captured in tags
* {{pagelink:Home/FHIR-Assets/Naming-Systems.page.md,text:Naming Systems}}
    * Changes to Identifiers
        * Consolidated BCUHBCentralPASIdentifier, BCUHBEastPASIdentifier and BCUHBWestPASIdentifier to BCUHBPASIdentifier
        
Guide:
* Added sections for FHIR Development Initiatives and Communities and FHIR Chat to {{pagelink:Home/Help-and-Support/Related-Pages.page.md,text:Related Pages}}
* Added a section for Change Requests to {{pagelink:Home/Help-and-Support/Help-and-Support.md,text:Help and Support}}.
* Created a new {{pagelink:Home/Design/Design-Patterns.page.md,text:Design Patterns}} page.
* Created a new {{pagelink:Home/Help-and-Support/Regular-Meetings.page.md,text:Regular Meetings}} page.
* Created a new {{pagelink:Home/Help-and-Support/Training.page.md,text:Training}} page.



### v1.1.1 STU1
Package:
* {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions,text:Profiles}}:
    * Changes to Profiles
        * DataStandardsWales-Provenance   
            * Updated references to use Data Standards Wales profiles     
* {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions,text:Extensions}}:
    * Changes to Extensions
        * DataStandardsWales-DemographicsAsRecorded
            * Renamed the DOB extension to birtDate 
            * Updated the extension URL
            * Updated the items within the extension URLs
        * DataStandardsWales-CDRPatientRecordType
            * Updated the name of the extension
        * DataStandardsWales-CDRSourceTimestamp
            * Updated the name of the extension

Guide:
* Updated the contact email address on the {{pagelink:Home/Help-and-Support/Related-Pages.page.md,text:Help and Support-Related Pages}}


            
### v1.1.0 STU1

Package: 
* {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions,text:Profiles}}:
    * New Profiles
        * DataStandardsWales-Device
        * DataStandardsWales-Provenance        
    * Changes to Profiles    
        * DataStandardsWales-Patient
            * Added Extensions for:
                * DataStandardsWales-CDRPatientRecordType
                * DataStandardsWales-CDRSourceTimestamp
* {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions,text:Extensions}}:
    * New Extensions
        * DataStandardsWales-CDRPatientRecordType
        * DataStandardsWales-CDRSourceTimestamp
        * DataStandardsWales-DemographicsAsRecorded

* {{pagelink:Home/FHIR-Assets/Terminology,text:Value Sets}}:
    * New Value Sets
        * DataStandardsWales-ProvenanceActivity
        * DataStandardsWales-PatientRecordType

 * {{pagelink:Home/FHIR-Assets/Naming-Systems.page.md,text:Naming Systems}}:
    * Corrected oid references. Changed from 2.16.840.1.113883.2.1.8.1.5.nnn to 2.16.840.1.113883.2.1.8.1.3.nnn    

Guide:
* Updated relevant pages within the Guide to reflect changes outlined in Package.
* Updated {{pagelink:Home/Help-and-Support/Glossary.page.md,text:Glossary}}.
  
* Added definitions for Active, Draft and Experimental to {{pagelink:Home/Introduction/Profile-Descriptions,text:Introduction-Profile Descriptions}}
* Added a link for FHIR PSOM Wales Project Page to {{pagelink:Home/Help-and-Support/Related-Pages.page.md,text:Help and Support-Related Pages}}
* Updated [Wales FHIR Implementation Guide Version History](https://simplifier.net/guide/Wales-FHIR-Implementation-Guide-Version-History-v1.1.0/Home/Version-History.page.md?version=1.1.0) to include links to respective Release Notes.


### v1.0.1 STU1

Package: 
* Profiles:
    * DataStandardsWales-Practitioner
        * Quotes removed from sdsuserid
    * DataStandardsWales-Location
        * Cardinality changed from 1..1 to 0..1:
            * .address
            * .managingOrganization.identifier
    * DataStandardsWales-MedicationDispense
        * Cardinality changed from 1..1 to 0..1:
            * .authorizingPrescription
            * .authorizingPrescription.reference
            * .identifier
            * .performer
            * .location.display
            * .quantity.value
            * .quantity.unit
            * .quantity.system
            * .quantity.code
        * Must support added to:
            * .location
            * .receiver
            * .context              
    * DataStandardsWales-Observation
        * Cardinality changed from 1..1 to 0..1:
            * .partOf.identifier
    * DataStandardsWales-Observation-Lab Resource
        * Corrected spelling error
* Code Systems:
    * DataStandardsWales-GenderIdentity
        * Trailing space removed from display value
    * DataStandardsWales-Sex
        * Trailing space removed from display value
* Value Set: 
    * DataStandardsWales-GenderIdentity
        * Trailing space removed from display value
    * DataStandardsWales-Sex
        * Trailing space removed from display value
    * DataStandardsWales-Title
        * Code expansion format corrected
* Concept Maps:
    * DataStandardsWales-GenderIdentity-HL7AdministrativeGender Resource
        * Corrected spelling error
        * Changed the targetURI to correct valueset
    * DataStandardsWales-HL7AdministrativeGender-GenderIdentity Resource
        * Changed the targetURI to correct valueset
    * DataStandardsWales-MaritalStatus-UKCorePersonMaritalStatusCode Resource
        * Changed the targetURI to correct valueset
        * Leading space removed from target value
* Extension:
    * DataStandardsWales-MedicationCourseOfTherapyType
        * Change to correct valueset
* Naming Systems:
    * Velindre PAS namespace OID corrected
    * BCUHB Central PAS Identifier corrected inconsistency
* Examples:
    * Organization - Glangwili General Hospital 
        * Removed hospital classification extension
    * Organization - Neath - Port Talbot Hospital 
        * Removed hospital classification extension
* Fixed render issues in ConceptsMaps, CodeSystem, NamingSystem & ValueSet by using HL7 FHIR XML element order
* Spaces removed in NamingSystems name to conform to HL7 as name can be used as id

Guide:
* DataStandardsWales-MedicationDispense
    * Mandatory and Must Support Data Elements list updated to reflect changes made to the profile and correct previously omitted information:
        * Updated the must have list as per current profile settings
        * Updated the must support list as per current profile settings   

### v1.0.0 STU1

* Changes made following feedback from the publication of the pre-release

### v1.0.0 STU1 - pre release

* Changes made in response to the ballot feedback process

### v0.1.1 STU1 - for ballot

* Minor errata to fix asset rendering issues

### v0.1.0 STU1 - for ballot

* First pass review of profiles
* Medication Scenarios
* Improvements to navigation
* Fixed page links and spelling
* Removed duplicate guidance
* References to HL7 or UK Core guidance where necessary


### 0.0.5 - Discovery

Experimental medication profiles were added.


* Immunization
* MedicationAdministration


The following experimental profiles were amended.


* MedicationDispense
* MedicationRequest


### 0.0.4 - Discovery

Experimental medication profiles were added.


* MedicationRequest
* MedicationDispense

A profile can now be designated as "Experimental" to show publishing intent in the near future.

### 0.0.2 & 0.0.3 - Discovery

Various profile drafts and fixes have been added.

### 0.0.1 - Discovery
The initial draft of the Data Standards Wales FHIR Implementation Guide, and should be considered 'under construction'. It contains only the base FHIR 'people and places' administrative resources.

This version is not intended for use, but is published for early comment and feedback.

<div class="container">
    <div class="row">
        <div class="col-md-7 card">
            <h4><b><a href="https://simplifier.net/guide/wales-fhir-implementation-guide-version-history" alt="Wales FHIR Implementation GUide Version History" target="_blank">Wales FHIR Implementation Guide Version History</a></b></h4>
            <p>Detailed description of the implementation guide changes</p>
        </div>
    </div>
</div>
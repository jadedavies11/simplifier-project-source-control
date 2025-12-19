## {{page-title}}

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
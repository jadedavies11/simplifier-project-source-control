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
* Value Sets:
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
* Extensions:
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
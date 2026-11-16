### v2.6.0 STU2

Package:
* Dependencies:
    * New Dependencies
        * hl7.fhir.uv.xver-r5.r4: 0.1.0
* Profiles and Extensions:
    * New Message Definitions
        * DataStandardsWales-CareDocumentSubmit
    * New Extensions
        * Extension-DataStandardsWales-AliasType
    * Removed Extensions
        * Extension-DataStandardsWales-DocumentAttester
        * Extension-DataStandardsWales-DocumentAttribute
        * Extension-DataStandardsWales-DocumentErrorAction
        * Extension-DataStandardsWales-DocumentErrorStatus
        * Extension-DataStandardsWales-DocumentVersion
        * Extension-DataStandardsWales-Immunization.basedOn
        * Extension-DataStandardsWales-SourceSystem
    * Changes to Profiles
        * DataStandardsWales-DocumentReference
            * Updated version from 0.1.0 to 1.0.0
            * .status. Updated from draft to active
            * extension:attesterR5. Removed Extension-DataStandardsWales-DocumentAttester
            * extension:attesterR5. Added http://hl7.org/fhir/5.0/StructureDefinition/extension-DocumentReference.attester to reflect formal R5 to R4 backport. Updated target profiles and descriptive elements (e.g. short, definition, comment)
            * extension:documentAttribute. Removed Extension-DataStandardsWales-DocumentAttribute. Replaced by use of meta.tag
            * extension:errorAction. Removed Extension-DataStandardsWales-DocumentErrorAction. Error handling approach not yet finalised
            * extension:errorStatus. Removed Extension-DataStandardsWales-DocumentErrorStatus. Not required
            * extension:sourceSystem. Removed Extension-DataStandardsWales-SourceSystem. Replaced by use of meta.source
            * extension:versionR5. Removed Extension-DataStandardsWales-DocumentVersion
            * extension:versionR5. Added http://hl7.org/fhir/5.0/StructureDefinition/extension-DocumentReference.version to reflect formal R5 to R4 backport. Updated descriptive elements (e.g. short, definition, comment)
        * DataStandardsWales-Immunization
            * Updated version from 1.2.0 to 1.3.0
            * extension:immunizationBasedOnR5. Removed Extension-DataStandardsWales-Immunization.basedOn
            * extension:immunizationBasedOnR5. Added http://hl7.org/fhir/5.0/StructureDefinition/extension-Immunization.basedOn  to reflect formal R5 to R4 backport. Updated target profiles and descriptive elements (e.g. short, definition, comment)
        * DataStandardsWales-Organization
            * Updated version from 1.1.1 to 1.2.0
            * .identifier slice odsOrganisationCode. Added a must support flag
            * .identifier slice gpClusterCode. To be deprecated and updated definition
            * .type. Added sector, domain, classification and subclassification slices with a must support flag and extensible value set bindings
            * .type. Removed ValueSet-UKCore-OrganizationType and added ValueSet-DataStandardsWales-OrganizationTypeExtended
            * .alias. Added Extension-DataStandardsWales-AliasType
            * .address. Added Extension-UKCore-AddressKey
            * .address.postaLCode. Removed Wales-specific guidance from definition
    * Changes to Extensions
        * Extension-DataStandardsWales-DocumentDigitalStatus
            * Updated version from 0.1.0 to 1.0.0
            * .status. Updated from draft to active
        * Extension-DataStandardsWales-SingleRecord-AllergiesListUpdated
            * Updated version from 1.0.0 to 1.0.1
            * .status. Updated from draft to active
* Terminology:
    * New Code Systems
        * DataStandardsWales-AliasType
        * DataStandardsWales-MessageEvent
        * DataStandardsWales-OrganizationClassification
        * DataStandardsWales-OrganizationDomain
        * DataStandardsWales-OrganizationSector
        * DataStandardsWales-OrganizationSubclassification
    * New Value Sets
        * DataStandardsWales-AliasType
        * DataStandardsWales-OrganizationClassification
        * DataStandardsWales-OrganizationDomain
        * DataStandardsWales-OrganizationSector
        * DataStandardsWales-OrganizationSubclassification
        * DataStandardsWales-OrganizationTypeExtended
    * Removed Code Systems
        * DataStandardsWales-DocumentAttribute
        * DataStandardsWales-DocumentErrorAction
        * DataStandardsWales-DocumentErrorStatus
    * Removed Value Sets
        * DataStandardsWales-DocumentAttribute
        * DataStandardsWales-DocumentErrorAction
        * DataStandardsWales-DocumentErrorStatus
    * Changes to Code Systems
        * DataStandardsWales-DocumentDigitalStatus
            * Updated version from 0.1.0 to 1.0.0
            * .status. Updated from draft to active
    * Changes to Value Sets
        * DataStandardsWales-DocumentCategory
            * Updated version from 0.1.0 to 1.0.0
            * .status. Updated from draft to active
        * DataStandardsWales-DocumentDigitalStatus
            * Updated version from 0.1.0 to 1.0.0
            * .status. Updated from draft to active
        * DataStandardsWales-DocumentType
            * Updated version from 0.1.0 to 1.0.0
            * .status. Updated from draft to active
        * DataStandardsWales-MessageEvent
            * Updated version from 0.1.0 to 0.2.0
            * Added DataStandardsWales-MessageEvent as a CodeSystem
* Naming Systems:
    * New Naming Systems
        * Namespace for LIMS1 TCL encounter identifier
        * Namespace for LIMS2 TCLe encounter identifier
        * Namespaces for PAS location identifiers
    * Changes to Naming Systems
        * Changes to .publisher, .responsible, .description, and .usage values for all Naming Systems to align published naming conventions
* Examples:
    * New Examples
        * Example-DataStandardsWales-Bundle-CareDocumentSubmit-CDR
        * Example-DataStandardsWales-Location-GGH
        * Example-DataStandardsWales-Location-GGH-OPD
        * Example-DataStandardsWales-Organization-AmmanGwendraeth
        * Example-DataStandardsWales-Organization-AmmanTawe
        * Example-DataStandardsWales-Organization-CAVUHB
        * Example-DataStandardsWales-Organization-CardiffNorth
        * Example-DataStandardsWales-Organization-MedicalInsurer
        * Example-DataStandardsWales-Organization-NCMC
        * Example-DataStandardsWales-Organization-UHW
        * Example-DSW-DocumentReference-ExpiredInsuranceCover
        * Example-DSW-Encounter-DocumentedEvent-DiabetesConsultation
        * Example-DSW-PractitionerRole-Consultant-JoeBloggs-HDUHB
        * Example-DSW-PractitionerRole-Dietitian-JudeFrancis-HDUHB
        * Example-DSW-PractitionerRole-Nurse-EmilyMay-HDUHB
        * Example-DSW-Practitioner-Consultant-JoeBloggs
        * Example-DSW-Practitioner-Dietitian-JudeFrancis
        * Example-DSW-Practitioner-Nurse-EmilyMay
    * Changes to Examples
        * Example-DataStandardsWales-AllergyIntolerance-Morphine
            * AllergyIntolerance.reaction.substance.code. Removed trailing white space from code
        * Example-DataStandardsWales-Bundle-UEC-Discharge-UHWEUMI
            * Condition.clinicalStatus. Added a value
        * Example-AuditEvent-CreateObservations
            * AuditEvent.source. Added a value
        * Example-DataStandardsWales-Bundle-UEC-Triage-UHWEUMI
            * Condition.clinicalStatus. Added a value
        * Example-DataStandardsWales-DocumentReference-EncounterBased
            * DocumentReference.context.practiceSetting. Corrected to use the required binding
            * DocumentReference.extension:attesterR5. Corrected extension url from https://fhir.nhs.wales/StructureDefinition/Extension-DataStandardsWales-DocumentAttester to http://hl7.org/fhir/5.0/StructureDefinition/extension-DocumentReference.attester
            * DocumentReference.extension:documentAttribute. All entries removed and replaced by meta.tag
            * DocumentReference.extension:sourceSystem. Entry removed and replaced by meta.source
            * DocumentReference.extension:versionR5. Corrected extension url from https://fhir.nhs.wales/StructureDefinition/Extension-DataStandardsWales-DocumentVersion to http://hl7.org/fhir/5.0/StructureDefinition/extension-DocumentReference.version
            * DocumentReference.meta.source. Added a value
            * DocumentReference.meta.tag. One entry added per removed extension:documentAttribute entry, plus docattr_documenttypecode
            * Referenced examples adjusted
        * Example-DataStandardsWales-DocumentReference-EventBased
            * DocumentReference.context.practiceSetting. Corrected to use the required binding
            * DocumentReference.extension:attesterR5. Corrected extension url from https://fhir.nhs.wales/StructureDefinition/Extension-DataStandardsWales-DocumentAttester to http://hl7.org/fhir/5.0/StructureDefinition/extension-DocumentReference.attester
            * DocumentReference.extension:documentAttribute. All entries removed and replaced by meta.tag
            * DocumentReference.extension:sourceSystem. Entry removed and replaced by meta.source
            * DocumentReference.extension:versionR5. Corrected extension url from https://fhir.nhs.wales/StructureDefinition/Extension-DataStandardsWales-DocumentVersion to http://hl7.org/fhir/5.0/StructureDefinition/extension-DocumentReference.version
            * DocumentReference.meta.source. Added a value
            * DocumentReference.meta.tag. One entry added per removed extension:documentAttribute entry, plus docattr_documenttypecode
            * Referenced examples adjusted
        * Example-DataStandardsWales-DocumentReference-NotEventBased
            * DocumentReference.extension:sourceSystem. Entry removed and replaced by meta.source
            * DocumentReference.meta.source. Added a value
            * DocumentReference.meta.tag. One entry added for docattr_documenttypecode
            * Referenced examples adjusted
        * Example-DataStandardsWales-Immunization-FluVaccine
            * Immunization.performer.actor.type. Added a value
        * Example-DataStandardsWales-Immunization-NotGiven
            * Immunization.vaccineCode.coding.code. Added a value
        * Example-DataStandardsWales-Organization-GGH
            * Added .type and .alias entries
            * Corrected .partOf reference
            * Removed trailing spaces
        * Example-DataStandardsWales-Organization-HDUHB
            * Added .type and .alias entries
            * Removed trailing spaces
        * Example-DataStandardsWales-Organization-NPT
            * Added .type and .alias entries
            * Corrected .partOf reference
            * Removed trailing spaces
        * Example-DataStandardsWales-Organization-SBUHB
            * Added .type and .alias entries
            * Removed trailing spaces
        * Example-DataStandardsWales-Patient-HaroldJames
            * Patient.extension:religion.value. Updated the value to match sample data in ValueSet-DataStandardsWales-Religion
        * Example-DataStandardsWales-PractitionerRole-Consultant
            * Corrected .organization reference
        * Example-DataStandardsWales-PractitionerRole-Consultant
            * Corrected .organization reference
        * Example-DataStandardsWales-PractitionerRole-Physiotherapist
            * Corrected .organization reference
        * Example-DataStandardsWales-PractitionerRole-PrescribingNurse
            * Corrected .organization reference
        * Example-WelshClinicalPortal-growth-chart-bundle
            * Bundle.meta.profile. Removed element.
    * Removed Examples
        * Example-DataStandardsWales-DocumentReference-MisfiledNotEventBased
            * Removed pending decisions on error workflow handling
        * Example-DataStandardsWales-Organization-GPCluster
            * Replaced by Example-DataStandardsWales-Organization-AmmanGwendraeth
        * Example-DataStandardsWales-Organization-GPPractice
            * Replaced by Example-DataStandardsWales-Organization-AmmanTawe
* Naming Conventions:
    * Added Naming Conventions for Message Definition Resources section

Guide:
* General improvements to IG that include fixing spelling mistakes, correcting grammatical errors and formatting, and correcting hyperlinks
* Added new pages to outline the Code Systems created in this release
* Added new pages to outline the Extensions created in this release
* Added new pages to outline the Examples created in this release
* Added new pages to outline the Message Definitions created in this release
* Added new pages to outline the Value Sets created in this release
* Added new page for Backport Extensions in FHIR Assets to list backport extensions used in the Data Standards Wales FHIR Implementation Guide
* Added new page for Dependencies History to our [Version History IG](https://simplifier.net/guide/Wales-FHIR-Implementation-Guide-Version-History/) page
* Updated Administrative Data guidance page to reflect the new Organization examples
* Updated Care Documents guidance page to clarify the potential roles of Device, Patient, RelatedPerson, Practitioner and PractitionerRole
* Updated Care Documents guidance page to indicate the implementation of encounter-based document metadata by the Care Documents Service
* Updated Care Documents guidance page to indicate the use of meta tags to store legacy document attributes
* Updated Care Documents guidance page to replace Document Error Workflow section content with placeholder statements pending new guidance
* Updated Care Documents guidance page with a new section to outline care document versions handling differences between WCRS and FHIR
* Updated Care Documents guidance page with added examples
* Updated DataStandardsWales-DocumentReference profile page to reflect the revised set of extensions
* Updated DataStandardsWales-DocumentReference profile page with added examples
* Updated DataStandardsWales-DocumentReference profile page to remove Provenance-related example
* Updated DataStandardsWales-DocumentReference profile status to active in Resource Index
* Updated DataStandardsWales-Immunization profile page to reflect the revised set of extensions
* Updated DataStandardsWales-Location profile page with added examples
* Updated DataStandardsWales-Organization profile page to align narrative content with profile changes
* Updated DataStandardsWales-Organization profile page with added examples
* Updated DataStandardsWales-Practitioner profile page with added examples
* Updated DataStandardsWales-PractitionerRole profile page with added examples
* Updated DataStandardsWales-Provenance profile page to include provenance-related DocumentReference example
* Updated Deployment Help and Support page to provide a fuller description of the use of dependencies
* Updated DocumentReference example pages to provide a fuller description of the scenario
* Updated Naming Systems index page to split by organisation
* Removed pages relating to removed Code Systems
* Removed pages relating to removed Examples
* Removed pages relating to removed Extensions
* Removed pages relating to removed Value Sets
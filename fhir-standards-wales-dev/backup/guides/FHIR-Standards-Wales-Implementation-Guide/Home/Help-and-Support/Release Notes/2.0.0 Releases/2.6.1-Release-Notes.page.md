### v2.6.1 STU2 - Urgent Correction Release
Summary: This release contains urgent corrections to DocumentReference and related resources, discovered during early use by the NHS Wales Care Documents Service of the newly activated DataStandardsWales-DocumentReference profile in the Wales FHIR Implementation Guide v2.6.0. It also contains a correction of a misleading Practitioner identifier slice name for registered pharmacists.

Impact: No breaking changes: NOTE that the correction of the required value set binding for DocumentReference.practiceSetting would be a breaking change for any system applying the incorrect binding which was inadvertently introduced in version 2.6.0. However the Care Documents Service is expected to be the first user of the new Wales FHIR standard for care documents, and will use the corrected resource definition when they start processing documents into the Care Data Repository.

Package:
* Profiles and Extensions:
    * Changes to Profiles
        * DataStandardsWales-DocumentReference
            * Updated version from 1.0.0 to 1.1.0
            * .context.practiceSetting. ValueSet binding amended from UKCore-PracticeSettingCode to UKCore-CareSettingType
            * .extension:versionR5. SetSequenceNumber statement removed from definition
            * .extension:versionR5.value. SetSequenceNumber statement removed from definition
            * .identifier.slicing.description. Updated to refer to Care Documents Service instead of WCRS
            * .identifier:wcrsDocumentId. Slice renamed as documentId; fixedUrl and definition adjusted accordingly
            * .identifier:wcrsSupersessionSetId. Slice renamed as supersessionSetId; fixedUrl and definition adjusted accordingly
            * .identifier:externalSupersessionSetId. Slice added
            * .identifier.system. min value set to 1 for all slices; examples added with realistic content for slice
            * .identifier.value. min value set to 1 for all slices; comments and examples added with realistic content for slice
        * DataStandardsWales-Practitioner
            * Updated version from 1.1.3 to 1.1.4
            * .identfiier:gphcCode. Slice renamed as :gphcNumber
* Naming Systems:
    * New Naming Systems
        * DataStandardsWales-document-identifier
        * DataStandardsWales-external-supersession-set-identifier
        * DataStandardsWales-supersession-set-identifier
    * Removed Naming Systems
        * DataStandardsWales-wcrs-document-identifier (replaced by DataStandardsWales-document-identifier)
        * DataStandardsWales-wcrs-supersession-set-identifier (replaced by DataStandardsWales-supersession-set-identifier)
* Examples:
    * Changes to Examples
        * Example-DataStandardsWales-Bundle-CareDocumentSubmit-CDR
            * .identifier. Entries adjusted to match latest slice definitions
            * .context.practiceSetting. Updated to use SNOMED CT binding
        * Example-DataStandardsWales-DocumentReference-EncounterBased
            * .identifier. Entries adjusted to match latest slice definitions
            * .context.practiceSetting. Updated to use SNOMED CT binding
        * Example-DataStandardsWales-DocumentReference-EventBased
            * .identifier. Entries adjusted to match latest slice definitions
            * .context.practiceSetting. Updated to use SNOMED CT binding
        * Example-DataStandardsWales-DocumentReference-ExpiredInsuranceCover
            * .identifier. Entries adjusted to match latest slice definitions
        * Example-DataStandardsWales-DocumentReference-NotEventBased
            * .identifier. Entries adjusted to match latest slice definitions

Guide:

* Updated Care Documents guidance to clarify the role of Welsh Care Records Service as legacy and remove inappropriate references
* Updated Care Documents guidance to remove statements indicating a preference for Encounter-based submission of event-related document metadata
* Updated DataStandardsWales-Practitioner profile page to reflect the revised set of identifier slices
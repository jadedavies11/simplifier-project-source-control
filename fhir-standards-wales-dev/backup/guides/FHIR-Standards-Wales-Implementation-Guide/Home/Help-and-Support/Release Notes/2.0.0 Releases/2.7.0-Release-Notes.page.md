### v2.7.0 STU2

In addition to general maintenance, this release includes enhancements to support:

* The Choose Pharmacy service
* Complex organisation and location structures, including type classifications, regions and clusters
* Error workflows for care documents

The release also introduces the [HL7 FHIR Translation Extension](http://hl7.org/fhir/StructureDefinition/translation) to the Data Standards Wales - Organization and Data Standards Wales - Location profiles, enabling the representation of Welsh-language translation of address fields sourced from Welsh Reference and Terminology Services (WRTS) databases

WITHDRAWN Assets: <br>
The following assets have been marked as withdrawn in this release and have a lifecycle status of retired. These will no longer be maintained within the Wales FHIR Implementation Guide or Wales FHIR package and SHALL NOT be used for new or revised content.
They will be removed from the next release of the Wales FHIR Implementation Guide and fhir.r4.wales 2.8.0 package

* .identifier slice gpClusterCode (DataStandardsWales-Organization)

DEPRECATED Assets:<br>
The following assets have been marked as deprecated in this release.
Deprecated assets are expected to be withdrawn in a future release unless otherwise stated. They remain available within the Wales FHIR Implementation Guide and fhir.r4.wales 2.8.0 package but SHOULD NOT be used for new or revised content. Instead, implementers should consider the identified alternatives, where provided.

* DataStandardsWales-UEC-MessageEvent code system. Any valid code system agreed with the receiving system can be used instead.
* GPClusterCode naming system. Use WRTSClusterCode naming system instead.
* MessageDefinition-DataStandardsWales-UEC-Arrival. Any valid message definition agreed with the receiving system can be used instead.
* MessageDefinition-DataStandardsWales-UEC-Discharge. Any valid message definition agreed with the receiving system can be used instead.
* MessageDefinition-DataStandardsWales-UEC-Triage. Any valid message definition agreed with the receiving system can be used instead.

Package:
* Updated structure definition meta data elements for contact information and copyright for various Profiles, Extensions, Code Systems and Value Sets to reflect current information.
* Dependencies:
    * Changes to Dependencies
        * fhir.r4.ukcore.stu2
            * Version updated from 2.0.1 to 2.0.2
* {{pagelink:Home/FHIR-Assets/Profile-Index.page.md,text:Profiles}}:
    * New Profiles
        * DataStandardsWales-HealthcareService
        * DataStandardsWales-OrganizationAffiliation
        * DataStandardsWales-Task
    * Changes to Profiles
        * DataStandardsWales-Appointment
            * Updated version from 1.2.1 to 1.2.2
            * .participant.actor. Updated reference from HL7 HealthcareService to DataStandardsWales-HealthcareService
        * DataStandardsWales-DocumentReference
            * Updated version from 1.1.0 to 1.1.1
            * .content.attachment.language. Removed references to ISO 639-3
        * DataStandardsWales-Encounter
            * Updated version from 1.0.3 to 1.0.4
            * .extension:Speciality. Updated element name to .extension:speciality
        * DataStandardsWales-ImagingStudy
            * Updated version from 0.2.1 to 0.3.0
            * .basedOn. Updated reference from HL7 Task to DataStandardsWales-Task
        * DataStandardsWales-Location
            * Updated version from 1.1.2 to 1.2.0
            * Added Extension-DataStandardsWales-GridReference
            * Added Extension-DataStandardsWales-LocationPeriod
            * .identifier:odsSiteCode. Re-enabled slice
            * .identifier:wrtsLocationIdentifier. Added Must Support
            * .identifier slice. Added glnCode
            * .identifier slice. Added gphcPremisesNumber
            * .identifier slice. Added nwsspPharmacyAccountNumber
            * .identifier slice. Added nhsbsaOpticianContractNumber
            * .identifier slice. Added bsaDentalLocationIdentifier
            * .name. Reverted cardinality to match UKCore
            * .name. Added Extension HL7 Translation
            * .alias. Added Extension-DataStandardsWales-AliasType
            * .type slice. Added locationCategory
            * .type slice. Added locationType
            * .address. Added Extension-UKCore-AddressKey
            * .physicalType. Added ValueSet-DataStandardsWales-LocationForm
        * DataStandardsWales-Organization
            * Updated version from 1.2.1 to 1.3.0
            * Added Extension-DataStandardsWales-SuccessorOrganization
            * .identifier slice. Added wrtsOrganizationIdentifier
            * .identifier slice gpClusterCode. To be withdrawn and updated definition
            * .name. Added Extension HL7 Translation
        * DataStandardsWales-Practitioner
            * Updated version from 1.1.4 to 1.2.0
            * .identifier. Added User Principal Name (UPN) slice
        * DataStandardsWales-PractitionerRole
            * Updated version from 1.1.3 to 1.1.4
            * .healthcareService. Updated reference from HL7 HealthcareService to DataStandardsWales-HealthcareService
        * DataStandardsWales-ServiceRequest
            * Updated version from 1.1.1 to 1.1.2
            * .performer. Updated reference from UKCore-HealthcareService to DataStandardsWales-HealthcareService
* {{pagelink:Home/FHIR-Assets/Extension-Index.page.md,text:Extensions}}:
    * New Extensions
        * Extension-DataStandardsWales-GridReference
        * Extension-DataStandardsWales-LocationPeriod
        * Extension-DataStandardsWales-SuccessorOrganization
    * Changes to Extensions
        * Extension-DataStandardsWales-AliasType
            * Updated version from 0.1.0 to 0.2.0
            * Updated DataType from CodeableConcept to Code
            * Updated Binding Strength from Preferred to Extensible
            * .context. Additional entry added for Location.alias element
        * Extension-DataStandardsWales-Speciality
            * Updated version from 1.0.1 to 1.1.0
            * Updated Binding Strength from Extensible to Preferred
* {{pagelink:Home/FHIR-Assets/CodeSystem-Index.page.md,text:CodeSystems}}:
    * New Code Systems
        * DataStandardsWales-LocationForm
        * DataStandardsWales-LocationType
        * DataStandardsWales-LocationTypeCategory
    * Changes to Code Systems
        * DataStandardsWales-AliasType
            * Updated version from 0.1.0 to 0.1.1
            * Added new code for trading-as
            * Added Welsh language equivalents for all codes
            * Updated definitions for Official name and Preferred name
        * DataStandardsWales-UEC-MessageEvent
            * Updated version from 0.0.1 to 0.1.0
            * Added HL7 extension structuredefinition-standards-status with value deprecated
            * .description. Updated to indicate that the resource is DEPRECATED
* {{pagelink:Home/FHIR-Assets/ValueSet-Index.page.md,text:ValueSets}}:
    * New Value Sets
        * DataStandardsWales-LocationForm
        * DataStandardsWales-LocationType
        * DataStandardsWales-LocationTypeCategory
        * DataStandardsWales-LocationTypeExtended
        * UKCore-SourceOfServiceRequest - v1.3.0 added pending UK Core STU3 release
    * Changes to Value Sets
        * DataStandardsWales-AliasType
            * Updated version from 0.1.0 to 0.1.1
            * .description updated to indicate availability of English and Welsh language alias types
        * DataStandardsWales-ProvenanceActivity
            * Updated version from 1.0.1 to 1.0.2
            * Updated expansion
        * DataStandardsWales-ObservationVitalSignsType
            * Updated version from 1.0.1 to 1.1.0
            * Added ValueSet-DataStandardsWales-BloodPressure-AverageSystolic
        * PASReferralSource
            * Updated version from 1.0.0 to 1.0.1
            * Updated SNOMED CT constraint to match ValueSet-UKCore-SourceOfServiceRequest amendments
* {{pagelink:Home/FHIR-Assets/Naming-Systems,text:Naming Systems}}:
    * New Naming Systems
        * Namespace for NHS Wales Shared Services Partnership (NWSSP) Pharmacy Account Number
        * Namespace for a composite identifier for an OrganizationAffiliation
        * Namespace for User Principal Name (UPN) identifier
        * Namespace for WRTS Cluster Code identifier
    * Changes to Naming Systems
        * All Naming Systems reformatted to 'pretty print' for readability and consistency.
        * DataStandardsWales-Application-Instance-Identifier
            * .usage. Updated from Patient Identity to Issuing authority
        * DataStandardsWales-ABUHB-PAS-Sub-Specialty-Identifier
            * .name. Updated to ABUHBPASSubSpecialtyIdentifier
        * DataStandardsWales-BCUHB-PAS-Identifier
            * filename. Renamed to NamingSystem-BCUHB-pas-identifier
            * .id. Updated to DataStandardsWales-BCUHB-PAS-PatientIdentifier
            * .name. Updated to BCUHBPASPatientIdentifier
        * DataStandardsWales-BCUHB-PAS-PractitionerIdentifier
            * filename. Renamed to NamingSystem-BCUHB-pas-practitioner-identifier
        * DataStandardsWales-BCUHB-PAS-Sub-Specialty-Identifier
            * .name. Updated to BCUHBPASSubSpecialtyIdentifier
        * DataStandardsWales-CAVUHB-PAS-Identifier
            * .id. Updated to DataStandardsWales-CAVUHB-PAS-PatientIdentifier
            * .name. Updated to CAVUHBPASPatientIdentifier
        * DataStandardsWales-CAVUHB-PAS-LocationIdentifier
            * .responsible. Updated from NHS Wales to Cardiff and Vale University Health Board
        * DataStandardsWales-CAVUHB-PAS-Sub-Specialty-Identifier
            * .name. Updated to CAVUHBPASSubSpecialtyIdentifier
        * DataStandardsWales-CTMUHB-PAS-Identifier
            * .id. Updated to DataStandardsWales-CTMUHB-PAS-PatientIdentifier
            * .name. Updated to CTMUHBPASPatientIdentifier
        * DataStandardsWales-CTMUHB-PAS-Sub-Specialty-Identifier
            * .name. Updated to CTMUHBPASSubSpecialtyIdentifier
        * DataStandardsWales-GPCluster-Code
            * Deprecated Naming System. Use DataStandardsWales-WRTS-Cluster-Code instead.
        * DataStandardsWales-HDUHB-PAS-Identifier
            * .id. Updated to DataStandardsWales-HDUHB-PAS-PatientIdentifier
            * .name. Updated to HDUHBPASPatientIdentifier
        * DataStandardsWales-HDUHB-PAS-Sub-Specialty-Identifier
            * .name. Updated to HDUHBPASSubSpecialtyIdentifier
        * DataStandardsWales-LIMS-identifier
            * .usage. Updated from LIMS identity to Patient identity
        * NHSWales-LIMS-TCL-Report
            * filename. Renamed to NamingSystem-LIMS-TCL-report-identifier
        * NHSWales-LIMS-TCL-Report-Code
            * filename. Renamed to NamingSystem-LIMS-TCL-report-code-identifier
        * NHSWales-LIMS-TCLe-Report
            * filename. Renamed to NamingSystem-LIMS-TCLe-report-identifier
        * NHSWales-LIMS-TCLe-Report-Code
            * filename. Renamed to NamingSystem-LIMS-TCLe-report-code-identifier
        * DataStandardsWales-NADEX-identifier
            * .usage. Updated from Organization identity to Practitioner identity
        * DataStandardsWales-PTHB-PAS-Identifier
            * .id. Updated to DataStandardsWales-PTHB-PAS-PatientIdentifier
            * .name. Updated to PTHBPASPatientIdentifier
        * DataStandardsWales-PTHB-PAS-Sub-Specialty-Identifier
            * .name. Updated to PTHBPASSubSpecialtyIdentifier
        * DataStandardsWales-SBUHB-PAS-Identifier
            * .id. Updated to DataStandardsWales-SBUHB-PAS-PatientIdentifier
            * .name. Updated to SBUHBPASPatientIdentifier
        * DataStandardsWales-SBUHB-PAS-Sub-Specialty-Identifier
            * .name. Updated to SBUHBPASSubSpecialtyIdentifier
        * DataStandardsWales-VUNHST-Canisc-Identifier
            * .id. Updated to DataStandardsWales-VUNHST-Canisc-PatientIdentifier
            * .name. Updated to VUNHSTCaniscPatientIdentifier
        * DataStandardsWales-VUNHST-PAS-Identifier
            * .id. Updated to DataStandardsWales-VUNHST-PAS-PatientIdentifier
            * .name. Updated to VUNHSTPASPatientIdentifier
        * DataStandardsWales-VUNHST-PAS-Sub-Specialty-Identifier
            * .name. Updated to VUNHSTPASSubSpecialtyIdentifier
        * DataStandardsWales-WRTS-Cluster-Code
            * Removed UTF Encoding statement
        * DataStandardsWales-WRTS-Organization-identifier
            * Re-enabled Naming System
            * .usage. Updated from Do not use to Organization identity
* {{pagelink:Home/FHIR-Assets/Message-Definition-Index.page.md,text:Message Definitions}}
    * Changes to Message Definitions
        * MessageDefinition-DataStandardsWales-UEC-Arrival
            * Updated version from 0.1.0 to 0.2.0
            * Added HL7 extension structuredefinition-standards-status with value deprecated
            * .description. Updated to indicate that the resource is DEPRECATED
        * MessageDefinition-DataStandardsWales-UEC-Discharge
            * Updated version from 0.1.0 to 0.2.0
            * Added HL7 extension structuredefinition-standards-status with value deprecated
            * .description. Updated to indicate that the resource is DEPRECATED
        * MessageDefinition-DataStandardsWales-UEC-Triage
            * Updated version from 0.1.0 to 0.2.0
            * Added HL7 extension structuredefinition-standards-status with value deprecated
            * .description. Updated to indicate that the resource is DEPRECATED
* {{pagelink:Home/Example-Index.page.md,text:Examples}}:
    * New Examples
        * Example-DataStandardsWales-DocumentReference-Misfiled
        * Example-DataStandardsWales-DocumentReference-MisfileRejected
        * Example-DataStandardsWales-DocumentReference-PotentiallyMisfiled
        * Example-DataStandardsWales-DocumentReference-Revoked
        * Example-DataStandardsWales-Location-AmmanTawePartnership
        * Example-DataStandardsWales-Location-BrynammanCommunity
        * Example-DataStandardsWales-Location-MeddygfaCwmamman
        * Example-DataStandardsWales-Organization-Region-SouthCentral
        * Example-DataStandardsWales-Task-MisfileAccepted
        * Example-DataStandardsWales-Task-MisfileRejected
        * Example-DataStandardsWales-Task-MisfileRequested
        * Example-DSW-OrganizationAffiliation-CC201-W00142
        * Example-DSW-OrganizationAffiliation-R3D8C-7A3
    * Changes to Examples
        * Example-DataStandardsWales-Bundle-CareDocumentSubmit-CDR.
            * Removed Encounter elements and moved these to DocumentReference.context to reflect operational patterns
            * .extension:attesterR5.extension:mode.valueCode. Updated binding to HL7 CodeSystem
        * Example-DataStandardsWales-Bundle-SubmitClinician-Literal
            * Renamed to Example-DataStandardsWales-Bundle-ClinicianSubmit-Literal
            * .focus.definition. Updated to Example-DataStandardsWales-MessageDefinition-ClinicianSubmit
            * eventCoding.code. Updated to clinician-submit from submit-clinician
            * eventCoding.display. Updated to Clinician submit from Submit clinician
        * Example-DataStandardsWales-Bundle-SubmitClinician-Logical
            * Renamed to Example-DataStandardsWales-Bundle-ClinicianSubmit-Logical
            * .focus.definition. Updated to Example-DataStandardsWales-MessageDefinition-ClinicianSubmit
            * eventCoding.code. Updated to clinician-submit from submit-clinician
            * eventCoding.display. Updated to Clinician submit from Submit clinician
        * Example-DataStandardsWales-DocumentReference-EncounterBased
            * .extension:attesterR5.extension:mode.valueCode. Updated binding to HL7 CodeSystem
            * .content.attachment.language. Updated code to en
        * Example-DataStandardsWales-DocumentReference-EventBased
            * .versionId. Added element
            * .extension:attesterR5.extension:mode.valueCode. Updated binding to HL7 CodeSystem
            * .docStatus. Updated to final
            * .content.attachment.language. Updated code to en
        * Example-DataStandards-Wales-DocumentReference-ExpiredInsurance
            * .content.attachment.language. Updated code to en
        * Example-DataStandards-Wales-DocumentReference-NotEventBased
            * .content.attachment.language. Updated code to en
        * Example-DataStandardsWales-Location-CadogWard
            * .text. Removed
            * .status. Updated to Active
            * .type. Added content for Clinical areas and Ward
            * .physicalType. Added content for Ward
            * .managingOrganization.reference. Updated to Organization/Example-DataStandardsWales-Organization-GGH
        * Example-DataStandardsWales-Location-GGH
            * .text. Removed
            * .extension.gridReference. Added extension
            * .status. Updated to Active
            * .extension.welshPreferredName. Added extension
            * .alias.extension. Added content for official-name. official-name-welsh, preferred-name and preferred-name-welsh
            * .type. Added content for Hospital
            * .address.line. Added Translation extension and Welsh translation
            * .address.city. Added content for Carmarthenshire
            * .address.city. Added Translation extension and Welsh translation
            * .address.district. Added Translation extension and Welsh translation
            * .address.country. Added content for Wales
            * .address.country. Added Translation extension and Welsh translation
            * .physicalType. Added content for Site
        * Example-DataStandardsWales-Location-GGH-OPD
            * .text. Removed
            * .type. Added content for Clinical areas and Outpatients clinic
            * .physicalType. Added content for Clinical area
        * Example-DataStandardsWales-Location-WardE
            * .text. Removed
            * .type. Added content for Clinical areas and Ward
            * .physicalType. Added content for Ward
        * Example-DataStandardsWales-MessageDefinition-SubmitClinician
            * Renamed to Example-DataStandardsWales-MessageDefinition-ClinicianSubmit
            * eventCoding.code. Updated to clinician-submit from submit-clinician
            * eventCoding.display. Updated to Clinician submit from Submit clinician
        * Example-DataStandardsWales-Organization-AmmanGwendraeth
            * .identifier. Added an additional identifier using WRTSOrganizationIdentifier Naming System
            * .identifier. Updated Naming System from GPClusterCode to WRTSClusterCode
            * .text. Removed
            * .partOf.identifier. Removed
        * Example-DataStandardsWales-Organization-AmmanTawe
            * Added mainLocation extension content referencing Location/Example-DataStandardsWales-Location-AmmanTawePartnership
            * .identifier. Added an additional identifier using WRTSOrganizationIdentifier Naming System
            * .text. Removed
            * .name. Added HL7 Translation extension
            * .alias. Added Welsh aliases
            * .address.line. Added HL7 Language extension and Welsh translation
            * .address.city. Added HL7 Language extension and Welsh translation
            * .address.district. Added HL7 Language extension and Welsh translation
            * .address.country. Added HL7 Language extension and Welsh translation
            * .partOf. Replaced Reference to Organization/Example-DataStandardsWales-Organization-AmmanGwendraeth (cluster)
                * .partOf.reference. Updated to Organization/Example-DataStandardsWales-Organization-HDUHB
                * .partOf.display. Updated to Hywel Dda University Local Health Board
                * .partOf.identifier. Removed
        * Example-DataStandardsWales-Organization-CardiffNorth
            * .identifier. Added an additional identifier using WRTSOrganizationIdentifier Naming System
            * .identifier. Updated Naming System from GPClusterCode to WRTSClusterCode
            * .text. Removed
            * .partOf.identifier. Removed
        * Example-DataStandardsWales-Organization-CAVUHB
            * .identifier. Added an additional identifier using WRTSOrganizationIdentifier Naming System
            * .text. Removed
            * .name. Added HL7 Translation extension
            * .alias. Added Welsh aliases
            * .address.line. Added HL7 Language extension and Welsh translation
            * .address.city. Added HL7 Language extension and Welsh translation
            * .address.district. Added HL7 Language extension and Welsh translation
            * .address.country. Added HL7 Language extension and Welsh translation
        * Example-DataStandardsWales-Organization-GGH
            * Added mainLocation extension content referencing Location/Example-DataStandardsWales-Location-GGH
            * .identifier. Added an additional identifier using WRTSOrganizationIdentifier Naming System
            * .text. Removed
            * .name. Added HL7 Translation extension
            * .alias. Added Welsh aliases
            * .address.line. Added HL7 Language extension and Welsh translation
            * .address.city. Added HL7 Language extension and Welsh translation
            * .address.district. Added HL7 Language extension and Welsh translation
            * .address.country. Added HL7 Language extension and Welsh translation
            * .partOf.identifier. Removed
        * Example-DataStandardsWales-Organization-HDUHB
            * .identifier. Added an additional identifier using WRTSOrganizationIdentifier Naming System
            * .text. Removed
            * .name. Added HL7 Translation extension
            * .alias. Added Welsh aliases
            * .address.line. Added HL7 Language extension and Welsh translation
            * .address.city. Added HL7 Language extension and Welsh translation
            * .address.district. Added HL7 Language extension and Welsh translation
            * .address.country. Added HL7 Language extension and Welsh translation
        * Example-DataStandardsWales-Organization-MedicalInsurer
            * .text. Removed
        * Example-DataStandardsWales-Organization-NCMC
            * identifier. Added an additional identifier using WRTSOrganizationIdentifier Naming System
            * .text. Removed
            * .name. Added HL7 Translation extension
            * .alias. Added Welsh aliases
            * .address.line. Added HL7 Language extension and Welsh translation
            * .address.city. Added HL7 Language extension and Welsh translation
            * .address.district. Added HL7 Language extension and Welsh translation
            * .address.country. Added HL7 Language extension and Welsh translation
            * .partOf. Replaced Reference to Organization/Example-DataStandardsWales-Organization-CardiffNorth (cluster)
                * .partOf.reference. Updated to Organization/Example-DataStandardsWales-Organization-CAVUHB
                * .partOf.display. Updated to Cardiff and Vale University Local Health Board
                * .partOf.identifier. Removed
        * Example-DataStandardsWales-Organization-NPT
            * .identifier. Added an additional identifier using WRTSOrganizationIdentifier Naming System
            * .text. Removed
            * .name. Added HL7 Translation extension
            * .alias. Added Welsh aliases
            * .address.line. Added HL7 Language extension and Welsh translation
            * .address.city. Added HL7 Language extension and Welsh translation
            * .address.district. Added HL7 Language extension and Welsh translation
            * .address.country. Added HL7 Language extension and Welsh translation
            * .partOf.identifier. Removed
        * Example-DataStandardsWales-Organization-SBUHB
            * .identifier. Added an additional identifier using WRTSOrganizationIdentifier Naming System
            * .text. Removed
            * .name. Added HL7 Translation extension
            * .alias. Added Welsh aliases
            * .alias. Removed display
            * .address.line. Added HL7 Language extension and Welsh translation
            * .address.city. Added HL7 Language extension and Welsh translation
            * .address.district. Added HL7 Language extension and Welsh translation
            * .address.country. Added HL7 Language extension and Welsh translation
        * Example-DataStandardsWales-Organization-UHW
            * .identifier. Added an additional identifier using WRTSOrganizationIdentifier Naming System
            * .text. Removed
            * .name. Added HL7 Translation extension
            * .alias. Added Welsh aliases
            * .address.line. Added HL7 Language extension and Welsh translation
            * .address.city. Added HL7 Language extension and Welsh translation
            * .address.district. Added HL7 Language extension and Welsh translation
            * .address.country. Added HL7 Language extension and Welsh translation
            * .partOf.identifier. Removed
        * Example-DataStandardsWales-Practitioner-Consultant
            * .identifier. Added UPN identifier
        * Example-DataStandardsWales-Practitioner-Consultant-JoeBloggs
            * .identifier. Added UPN identifier
        * Example-DataStandardsWales-Practitioner-Dietitian-JudeFrancis
            * .identifier. Added UPN identifier
        * Example-DataStandardsWales-Practitioner-Doctor
            * .identifier. Added UPN identifier
        * Example-DataStandardsWales-Practitioner-NonClinical
            * .identifier. Added UPN identifier
        * Example-DataStandardsWales-Practitioner-Nurse-EmilyMay
            * .identifier. Added UPN identifier
        * Example-DataStandardsWales-Practitioner-Physiotherapist
            * .identifier. Added UPN identifier
        * Example-DataStandardsWales-Practitioner-PrescribingNurse
            * .identifier. Added UPN identifier
    * Removed Examples
        * Urgent and Emergency Care
            * Example Message Bundle - UEC Arrival UHWEUMI (UHW Emergency Unit Minor Injuries)
            * Example Message Bundle - UEC Triage UHWEUMI (UHW Emergency Unit Minor Injuries)
            * Example Message Bundle - UEC Discharge UHWEUMI (UHW Emergency Unit Minor Injuries)

Guide:

* General improvements to IG that include fixing spelling mistakes, correcting grammatical errors and formatting, and correcting hyperlinks
* Added new pages to outline the Code Systems created in this release
* Added new pages to outline the Examples created in this release, and updated example links on relevant profile pages
* Added new pages to outline the Extensions created in this release
* Added new pages to outline the Value Sets created in this release
* Added a new page to outline the DataStandardsWales-HealthcareService profile
* Added a new page to outline the DataStandardsWales-OrganizationAffiliation profile
* Added a new page to outline the DataStandardsWales-OrganizationTypeExtended value set which was created in 2.6.0
* Added a new page to outline the DataStandardsWales-Task profile
* Corrected spelling error for DataStandardsWales-OrganizationSubclassification in 2.6.0 Release Notes and ValueSet yaml toc file
* Reformatted Release Notes to match upgraded FHIR Assets pages
* Removed all pages related to example resources removed at this release
* Removed the Urgent and Emergency Care guidance page
* Restored 2.6.0 release details to Version History page
* Restructured and extended scope of FHIR Assets pages
* Restructured and extended scope of Naming Conventions page
* Updated Change Notices page in the [Version History IG](https://simplifier.net/guide/Wales-FHIR-Implementation-Guide-Version-History/)
* Updated CodeSystem-DataStandardsWales-UEC-MessageEvent page to clarify that the resource is deprecated
* Updated DataStandardsWales-Location profile page to align narrative content with profile changes
* Updated DataStandardsWales-Observation-VitalSigns profile page with further guidance on dependencies
* Updated DataStandardsWales-Observation-VitalSigns-BMI profile page with further guidance on dependencies
* Updated DataStandardsWales-Observation-VitalSigns-BodyHeight profile page with further guidance on dependencies
* Updated DataStandardsWales-Observation-VitalSigns-BodyWeight profile page with further guidance on dependencies
* Updated DataStandardsWales-Organization profile page to align narrative content with profile changes
* Updated DataStandardsWales-Practitioner profile page with new slice
* Updated Example Index with new examples
* Updated Example Index. Example Location - Cadog Ward (GGH) renamed as Example Location - Glangwili General Hospital Cadog Ward
* Updated Example Index. Example Location - Outpatients Department (GGH) renamed as Example Location - Glangwili General Hospital Outpatients Department
* Updated Example Index. Example Location - Ward E (NPT) renamed as Example Location - Neath Port Talbot Hospital Ward E
* Updated Example Index. Example-DataStandardsWales-Bundle-SubmitClinician-Literal renamed as Example-DataStandardsWales-Bundle-ClinicianSubmit-Literal
* Updated Example Index. Example-DataStandardsWales-Bundle-SubmitClinician-Logical renamed as Example-DataStandardsWales-Bundle-ClinicianSubmit-Logical
* Updated Example Index. Example-DataStandardsWales-MessageDefinition-SubmitClinician renamed as Example-DataStandardsWales-MessageDefinition-ClinicianSubmit
* Updated FHIR Messaging page with amended example links and amended diagram links
* Updated Example-DataStandardsWales-Bundle-CareDocumentSubmit-CDR page to remove placeholder text regarding external supersession identifiers
* Updated Example-DataStandardsWales-Location-AmmanTawePartnership page with additional context for translated values.
* Updated Example-DataStandardsWales-Location-BrynammanCommunity page with additional context for translated values.
* Updated Example-DataStandardsWales-Location-GGH page with additional context for translated values.
* Updated Example-DataStandardsWales-Location-MeddygfaCwmamman page with additional context for translated values.
* Updated Example-DataStandardsWales-Organization-AmmanTawe page with additional context for translated values.
* Updated Example-DataStandardsWales-Organization-CAVUHB page with additional context for translated values.
* Updated Example-DataStandardsWales-Organization-GGH page with additional context for translated values.
* Updated Example-DataStandardsWales-Organization-HDUHB page with additional context for translated values.
* Updated Example-DataStandardsWales-Organization-NCMC page with additional context for translated values.
* Updated Example-DataStandardsWales-Organization-NPT page with additional context for translated values.
* Updated Example-DataStandardsWales-Organization-SBUHB page with additional context for translated values.
* Updated Example-DataStandardsWales-Organization-UHW page with additional context for translated values.
* Updated Extension-DataStandardsWales-AliasType page with additional use context of Location.alias
* Updated Guidance page for Administrative Data to cover additional resources and up-to-date advice on modelling structural relationships
* Updated Guidance page for Care Documents to cover error workflows and to clarify the data model scope and use of Encounter
* Updated Introduction-How to use this Implementation Guide page to indicate how to identify the HL7 FHIR release number used by these standards
* Updated MessageDefinition-DataStandardsWales-UEC-Arrival page to clarify that the resource is deprecated
* Updated MessageDefinition-DataStandardsWales-UEC-Discharge page to clarify that the resource is deprecated
* Updated MessageDefinition-DataStandardsWales-UEC-Triage page to clarify that the resource is deprecated
* Updated Resource Index by relocating DataStandardWales-Condition from Entities to Diagnostics
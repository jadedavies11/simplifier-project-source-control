## {{page-title}}

Package: 
* {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions,text:Profiles and Extensions}}:
    * New Profiles
        * DataStandardsWales-MessageDefinition
        * DataStandardsWales-MessageHeader
    * New Extensions 
    * New Message Definitions
        * MessageDefinition-DataStandardsWales-UEC-Arrival
    * Changes to Profiles
        * DataStandardsWales-MedicationRequest
            * Updated version from 1.2.0 to 1.3.0
            * .requestor. Cardinality changed from 1..1 to 0..1 to align with UKCore.
    * Changes to Extensions
* {{pagelink:Home/FHIR-Assets/Terminology,text:Terminology}}:
    * New Code Systems
        * DataStandardsWales-UEC-MessageEvent
    * Removed Code Systems
    * Changes to Code Systems
    * New Value Sets
        * DataStandardsWales-MessageEvent
    * Removed Value Sets
    * Changes to Value Sets
        * DataStandardsWales-EncounterType
            * Updated version from 1.0.0 to 1.1.0
            * Updated SNOMED CT 20250409 version 
            * Expanded SNOMED CT codes to show 50 concepts as sample
        * DataStandardsWales-Occupation
            * Updated version from 0.0.5 to 0.1.0
            * Updated SNOMED CT 20250409 version 
            * Expanded SNOMED CT codes to show 50 concepts as sample
        * DataStandardsWales-Occupation
            * Updated version from 1.0.0 to 1.1.0
            * Updated SNOMED CT 20250409 version 
            * Expanded SNOMED CT codes to show 50 concepts as sample
* {{pagelink:Home/FHIR-Assets/Naming-Systems.page.md,text:Naming Systems}}
    * Changes to Naming Systems
        * New Naming Systems
            * Namespaces for PAS link identifiers
* {{pagelink:Home/Example-Index.page.md,text:Examples}}:
    * New Examples
        * Urgent and Emergency Care
            * Example Message Bundle - UEC Arrival UHWEUMI (UHW Emergency Unit Minor Injuries)
        * FHIR Messaging guidance
            * Example Message Bundle - Submit Clinician (Logical Referencing)
            * Example Message Bundle - Submit Clinician (Literal FHIR Referencing)
            * Example Message Definition - Submit Clinician

Guide:
* General improvements to IG that include fixing spelling mistakes, correcting grammatical errors and formatting
* Added a new page to outline the DataStandardsWales-MessageDefinition profile
* Added a new page to outline the DataStandardsWales-MessageHeader profile
* Added new pages to outline the Message Definitions created in this release
* Added new pages to outline the Code Systems created in this release
* Added new pages to outline the Value Sets created in this release
* Added new pages to outline the Examples created in this release
* Added FHIR Messaging Guidance page
* Added Urgent and Emergency Care Guidance page (PLACEHOLDER)
* Added WRTS contact details to DataStandardsWales-EncounterType Value Set guide page
* Added WRTS contact details to DataStandardsWales-Occupation Value Set guide page
* Added WRTS contact details to DataStandardsWales-Religion Value Set guide page
* Removed duplicated examples from DataStandardsWales-Observation guide page. All examples are now located in the Examples tab of the Profile Content table
* Renamed Naming Systems page in Design tab to Naming Systems Design
* Updated page link in FHIR Assets Naming System from Naming System to Naming Systems Design
* Standardised resource links in IG pages
* Correct title page for Extension Data Standards Wales Speciality to align with IG standards
* Alphabetised yaml toc files
* Standardised examples names in Example Index page
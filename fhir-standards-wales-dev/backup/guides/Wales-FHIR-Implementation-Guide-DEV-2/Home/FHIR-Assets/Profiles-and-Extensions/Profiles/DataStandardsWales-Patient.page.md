<div class="warning"><span class="ImplementWarn"></span></div>

## {{page-title}}

### Overview
The [Patient](https://hl7.org/fhir/patient.html) resource contains demographics and other administrative information about an individual receiving health or care-related services.

The {{page-title}} profile is derived from the [UK Core Patient Profile](https://simplifier.net/guide/uk-core-implementation-guide/Home/ProfilesandExtensions/ProfileUKCore-Patient?version=1.0.0). It defines additional rules for use within health and care organisations in Wales.


### Formal Views of Profile Content
<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openCity(this,'tabsnap')" data-target="tabsnap">
      Snapshot View
    </li>
    <li class="tablink" onclick="openCity(this,'tabdiff')" data-target="tabdiff">
      Differential View
    </li>
    <li class="tablink" onclick="openCity(this,'tabhybrid')" data-target="tabhybrid">
      Hybrid View
    </li>
    <li class="tablink" onclick="openCity(this,'tabeg')" data-target="tabeg">
      Examples
    </li>     
  </ul>
  <div class="tab-main">
    <div id="tabsnap" class="tabcontent active">      
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Patient, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Patient, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Patient, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>{{pagelink:Example-DataStandardsWales-Patient-AliceJones, text:Example Patient - Alice Jones}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Patient-AliceJones, text:Example Patient - Harold James}}</li>
    </list>
  </div>   
</div>

### Mandatory and Must Support Data Elements
When an element is mandatory (min=1), the data is expected to always be present. Elements marked with an <span style="background-color:red;color:white;">S</span> must be supported by both producing and receiving systems and **SHOULD** be populated if the data exists.

Each Patient record must support:
* A patient identifier
   * This field **SHOULD** include at least one patient identifier:
   * NHS Numbers are to be be provided if available. Use the [UKCore-NHSNumberVerificationStatus](https://simplifier.net/guide/uk-core-implementation-guide/Home/ProfilesandExtensions/ExtensionLibrary?version=1.0.0#ExtensionUKCore-NHSNumberVerificationStatus) to indicate the trace status.contain all available identifiers. 
   * Other patient identifiers can also be included where known e.g., Welsh Demographic Service or Health Board PAS identifiers.
   * Identifier systems should use the NamingSystem URIs which are defined in the guide rather than OIDS.
* Address and contact information
* The status of the patient record (i.e., whether is still active )
* A deceased indicator

The following [Core Reference Data Standards](https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm) defines standards for the following elements, which are also marked as must be supported:
* religion
* language 
* ethnicity
* postcode
* marital status*
* sex*
* gender*

\* When populating these fields implementers are required to use the codes defined by HL7. Concept maps are provided below to indicate required mappings to and from Wales codes for gender identity, sex and marital status as defined in the [Core Reference Data Standards](https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm) published by the Welsh Information Standards Board.

### Extensions

The extensions listed below are those created to support Data Standards Wales: 

* DataStandardsWales-Religion defined in the [NHS Wales Data Dictionary](https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm).
* DataStandardsWales-Occupation Patient.extension:occupation this uses a SNOMED  CT reference set.


_Note: this list does not include extensions provided by UK Core and you should refer to their implementation guide for support_

### Slices
The following identifier slices for use with the patient profile are listed below. The namespaces denoting issuing authority for each identifier are defined on the {{pagelink:Home/FHIR-Assets/Naming-Systems.page.md, text:Naming Systems}} page.  NHS numbers are further described in the [NHS Wales Data Dictionary](https://www.datadictionary.wales.nhs.uk/).
 
* `Patient.identifier:nhsNumber` 
* `Patient.identifier:abuhbPasIdentifier` 
* `Patient.identifier:bcuhbCentralPasIdentifier`  
* `Patient.identifier:bcuhbEastPasIdentifier` 
* `Patient.identifier:bcuhbWestPasIdentifier` 
* `Patient.identifier:cavuhbPasIdentifier` 
* `Patient.identifier:ctmuhbPasIdentifier` 
* `Patient.identifier:hduhbPasIdentifier` 
* `Patient.identifier:pthbPasIdentifier` 
* `Patient.identifier:sbuhbPasIdentifier` 
* `Patient.identifier:vunhstCaniscIdentifier` 

### Terminology Bindings (differential)
This profile defines the following terminology bindings in addition to those defined in UK Core.

* {{pagelink:Home/FHIR-Assets/Terminology/Value-Sets/ValueSet-DataStandardsWales-Occupation.page.md, text:ValueSet-DataStandardsWales-Occupation}}
* {{pagelink:Home/FHIR-Assets/Terminology/Value-Sets/ValueSet-DataStandardsWales-Title.page.md, text:ValueSet-DataStandardsWales-Title}}
* {{pagelink:Home/FHIR-Assets/Terminology/Value-Sets/ValueSet-DataStandardsWales-Religion.page.md, text:ValueSet-DataStandardsWales-Religion}}

### Concept Maps
The following concept maps provide a mapping to and from UK Core / HL7 codes to Data Standards Wales codes:

|Concept|Mapping for HL7/UK Core codes to Data Standards Wales codes|Mapping for Data Standards Wales codes to HL7/UK Core codes|
|-|-|-|
|Marital status|{{pagelink:Home/FHIR-Assets/Terminology/Concept-Maps/ConceptMap-DataStandardsWales-UKCorePersonMaritalStatusCode-MaritalStatus.page.md, text:DataStandardsWales-UKCorePersonMaritalStatusCode-MaritalStatus}}|{{pagelink:Home/FHIR-Assets/Terminology/Concept-Maps/ConceptMap-DataStandardsWales-MaritalStatus-UKCorePersonMaritalStatusCode.page.md, text:DataStandardsWales-MaritalStatus-UKCorePersonMaritalStatusCode}}|
|Gender identity|{{pagelink:Home/FHIR-Assets/Terminology/Concept-Maps/ConceptMap-DataStandardsWales-HL7AdministrativeGender-GenderIdentity.page.md, text:DataStandardsWales-HL7AdministrativeGender-GenderIdentity}}|{{pagelink:Home/FHIR-Assets/Terminology/Concept-Maps/ConceptMap-DataStandardsWales-GenderIdentity-HL7AdministrativeGender.page.md, text:DataStandardsWales-GenderIdentity-HL7AdministrativeGender}}|
|Sex|{{pagelink:Home/FHIR-Assets/Terminology/Concept-Maps/ConceptMap-DataStandardsWales-UKCoreBirthSex-Sex.page.md, text:DataStandardsWales-UKCoreBirthSex-Sex}}|{{pagelink:Home/FHIR-Assets/Terminology/Concept-Maps/ConceptMap-DataStandardsWales-Sex-UKCoreBirthSex.page.md, text:DataStandardsWales-Sex-UKCoreBirthSex}}|
<div class="warning"><span class="ImplementWarn"></span></div>

## {{page-title}}

### Overview
The [Patient](https://www.hl7.org/fhir/r4/patient.html) resource contains demographics and other administrative information about an individual receiving health or care-related services.

The {{page-title}} profile is derived from the [UK Core Patient Profile](https://simplifier.net/guide/uk-core-implementation-guide-stu2/Home/ProfilesandExtensions/Profile-UKCore-Patient?version=2.0.1). It defines additional rules for use within health and care organisations in Wales.

A direct link to the Data Standards Wales asset can be accessed here - {{link:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Patient}}


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
      <li>{{pagelink:Example-DataStandardsWales-Patient-HaroldJames, text:Example Patient - Harold James}}</li>
    </list>
  </div>   
</div>

### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Mandatory-and-Must-Support-Data-Elements,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.

Each Patient record must support:
* A patient identifier
   * This field **SHOULD** include at least one patient identifier:
   * NHS Numbers are to be be provided if available. Use the [UKCore-NHSNumberVerificationStatus](https://simplifier.net/guide/uk-core-implementation-guide-stu2/Home/ProfilesandExtensions/ExtensionLibrary/Extension-UKCore-NHSNumberVerificationStatus?version=2.0.1) to indicate the trace status.contain all available identifiers. 
   * Other patient identifiers can also be included where known e.g., Welsh Demographic Service or Health Board PAS identifiers.
   * Identifier systems should use the NamingSystem URIs which are defined in the guide rather than OIDS.
* Address and contact information
* The status of the patient record (i.e. whether is still active )
* A deceased indicator

The following elements are defined by [Core Reference Data Standards](https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm), which are also marked as must be supported:

* religion
* language 
* ethnicity
* postcode
* marital status*
* sex*
* gender*

When populating these fields implementers are required to use the codes defined by HL7. Concept maps are provided below to indicate required mappings to and from Wales codes for gender identity, sex and marital status as defined in the [Core Reference Data Standards](https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm) published by the Welsh Information Standards Board.

### Extensions

The extensions listed below are those created to support Data Standards Wales: 

* {{pagelink:Extension-DataStandardsWales-Religion,text:DataStandardsWales-Religion}}
  defined in the [NHS Wales Data Dictionary](https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm).
* {{pagelink:Extension-DataStandardsWales-Occupation,text:DataStandardsWales-Occupation}} indicates the patient occupation and uses a SNOMED  CT reference set.


_Note: this list does not include extensions provided by UK Core and you should refer to their implementation guide for support_

### Slices
The following identifier slices for use with the patient profile are listed below. The namespaces denoting issuing authority for each identifier are defined on the {{pagelink:Naming-Systems, text:Naming Systems}} page.  NHS numbers are further described in the [NHS Wales Data Dictionary](https://www.datadictionary.wales.nhs.uk/).
 
* `Patient.identifier:nhsNumber` 
* `Patient.identifier:abuhbPasIdentifier` 
* `Patient.identifier:bcuhbPasIdentifier`  
* `Patient.identifier:cavuhbPasIdentifier` 
* `Patient.identifier:ctmuhbPasIdentifier` 
* `Patient.identifier:hduhbPasIdentifier` 
* `Patient.identifier:pthbPasIdentifier` 
* `Patient.identifier:sbuhbPasIdentifier` 
* `Patient.identifier:vunhstCaniscIdentifier` 

### Terminology Bindings (differential)
This profile defines the following terminology bindings in addition to those defined in UK Core.

* {{pagelink:ValueSet-DataStandardsWales-Occupation, text:ValueSet-DataStandardsWales-Occupation}}
* {{pagelink:ValueSet-DataStandardsWales-Title, text:ValueSet-DataStandardsWales-Title}}
* {{pagelink:ValueSet-DataStandardsWales-Religion, text:ValueSet-DataStandardsWales-Religion}}

### Concept Maps
The following concept maps provide a mapping to and from UK Core / HL7 codes to Data Standards Wales codes:

|Concept|Mapping for HL7/UK Core codes to Data Standards Wales codes|Mapping for Data Standards Wales codes to HL7/UK Core codes|
|-|-|-|
|Marital status|{{pagelink:ConceptMap-DataStandardsWales-UKCorePersonMaritalStatusCode-MaritalStatus, text:DataStandardsWales-UKCorePersonMaritalStatusCode-MaritalStatus}}|{{pagelink:ConceptMap-DataStandardsWales-MaritalStatus-UKCorePersonMaritalStatusCode, text:DataStandardsWales-MaritalStatus-UKCorePersonMaritalStatusCode}}|
|Gender identity|{{pagelink:ConceptMap-DataStandardsWales-HL7AdministrativeGender-GenderIdentity, text:DataStandardsWales-HL7AdministrativeGender-GenderIdentity}}|{{pagelink:ConceptMap-DataStandardsWales-GenderIdentity-HL7AdministrativeGender, text:DataStandardsWales-GenderIdentity-HL7AdministrativeGender}}|
|Sex|{{pagelink:ConceptMap-DataStandardsWales-UKCoreBirthSex-Sex, text:DataStandardsWales-UKCoreBirthSex-Sex}}|{{pagelink:ConceptMap-DataStandardsWales-Sex-UKCoreBirthSex, text:DataStandardsWales-Sex-UKCoreBirthSex}}|
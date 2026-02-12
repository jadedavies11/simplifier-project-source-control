<div class="warning"><span class="ImplementWarn"></span></div>

## {{page-title}}

### Overview

The [Organization](https://www.hl7.org/fhir/r4/organization.html) resource contains information about health and care organisations. Examples include Health Boards and NHS Trusts, Hospitals, Dental practices GP practices and GP clusters.  The {{page-title}} profile is derived from the [UK Core Organization Profile](https://simplifier.net/guide/uk-core-implementation-guide-stu2/Home/ProfilesandExtensions/Profile-UKCore-Organization?version=2.0.1). It defines additional rules for use within health and care organisations in Wales. Further guidance on the use of the Organization resource along with other administrative FHIR resources is provided within the {{pagelink:Home/Guidance/Administrative-Data, text: guidance}} section of this guide.

A direct link to the Data Standards Wales asset can be accessed here - {{link:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Organization}}

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Organization, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Organization, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Organization, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>{{pagelink:Example-DataStandardsWales-Organization-GGH, text: Glangwili General Hospital}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Organization-NPT, text: Neath Port Talbot Hospital}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Organization-HDUHB, text: Hywel Dda University Local Health Board}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Organization-SBUHB, text: Swansea Bay University Local Health Board}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Organization-GPPractice, text: GP Practice example}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Organization-GPCluster, text: GP Cluster example}}</li>
    </list>
  </div>
</div>

### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Mandatory-and-Must-Support-Data-Elements,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.

Each Organisation must have:
* A name
  * The `Organization.name` field **SHALL** be populated.

Each Organisation must support:
* An identifier*
  * The `Organization.identifier` field **SHOULD** contain all available identifiers. In particular:
    * The [Organisation Data Service](https://digital.nhs.uk/services/organisation-data-service) (ODS) issues and manages unique identification codes and accompanying reference data for organisations that interact with any area of the NHS. The ODS code for organisations managed by this service **SHOULD** be populated (this includes ANANA format codes).  <br /><br />

* The active status of the organisation
  * The `Organization.active` field **SHOULD** be populated to indicate whether the organisation is still active.  <br /><br />

* Details of `Organization.type`, ideally structured to comprise sector plus a hierarchical organization type 
  * `sector` **SHOULD** be provided to distinguish public, private and third sector organizations
  * `domain` **SHOULD** be provided to identify the domain or industry in which the organization operates
  * `classification` **SHOULD** be provided as a high level classification of the organization type within the applicable domain.
  * `subclassification` **SHOULD** be provided as a lower level classification of the organization type within the applicable domain.  <br /><br />

* For each `Organization.alias`, an `aliasType` extension **SHOULD** specify the nature of the alias.

* Where applicable:
  * the `Organization.partOf` field **SHOULD** contain a reference to the parent organization
  * the `Organization.telecon` field **SHOULD** contain at least one contact point (e.g. telephone number)
  * the `Organization.address` field **SHOULD** contain at least one address for the organization

_*See implementation guidance for the identifier element in the Slices section below_

### Extensions

The following extensions are defined for use within this profile: 
* The UK Core extension [Extension-UKCore-MainLocation](https://simplifier.net/guide/uk-core-implementation-guide-stu2/Home/ProfilesandExtensions/ExtensionLibrary/Extension-UKCore-MainLocation?version=2.0.1) extends the Organization resource to support the exchange of information on the Organisation's main location, as a reference to a Location resource, which is currently not supported by the FHIR standard.

* The UK Core extension [Extension-UKCore-AddressKey](https://simplifier.net/resolve?scope=package:fhir.r4.ukcore.stu2@2.0.1&filepath=package/Extension-UKCore-AddressKey.json) extends the Address datatype to support the storage of additional address identifiers.

* The HL7 common extension [organization-period](http://hl7.org/fhir/R4/extension-organization-period.html) describes the date range that the organization should be considered available.

* {{pagelink:Extension-DataStandardsWales-AliasType}} is used to specify the nature of each alias.
  
### Slices

Slices apply to the following elements:
* `Organization.identifier` 
  * `Organization.identifier:odsOrganisationCode`. The ODS Organisation Code is further described here: [UK Core Naming System](https://simplifier.net/guide/UKNamingSystems/Home?version=current)
  * `Organization.identifier:gpClusterCode`. This slice is marked as deprecated because it applies to only a small proportion of organizations and is misnamed for its current use. The identifier for a primary care cluster can be recorded as a generic identifier distinguished by its system value. It is further described under the GP Cluster Code entry in the [NHS Wales Data Dictionary](https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm).  <br /><br />

* `Organization.type` includes a slice for each of the four organization type variants described above under Mandatory and Must Support Data Elements: 
  * `Organization.type:sector`
  * `Organization.type:domain`
  * `Organization.type:classification`
  * `Organization.type:subclassification` 

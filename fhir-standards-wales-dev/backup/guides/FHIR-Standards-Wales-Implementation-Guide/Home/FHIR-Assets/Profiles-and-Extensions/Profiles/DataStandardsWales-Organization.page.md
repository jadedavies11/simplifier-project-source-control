## {{page-title}}

### Overview

The [Organization](https://www.hl7.org/fhir/R4/organization.html) resource contains information about health and care organisations. Examples include Health Boards and NHS Trusts, Hospitals, Dental practices GP practices and GP clusters.  The {{page-title}} profile is derived from the [UK Core Organization Profile](https://simplifier.net/guide/uk-core-implementation-guide-stu2/Home/ProfilesandExtensions/Profile-UKCore-Organization?version=2.0.1). It defines additional rules for use within health and care organisations in Wales. Further guidance on the use of the Organization resource along with other administrative FHIR resources is provided within the {{pagelink:Home/Guidance/Administrative-Data, text: guidance}} section of this guide.

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
      <li>{{pagelink:Example-DataStandardsWales-Organization-CAVUHB, text: Cardiff and Vale University Local Health Board}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Organization-HDUHB, text: Hywel Dda University Local Health Board}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Organization-SBUHB, text: Swansea Bay University Local Health Board}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Organization-UHW, text: University Hospital of Wales}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Organization-GGH, text: Glangwili General Hospital}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Organization-NPT, text: Neath Port Talbot Hospital}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Organization-CardiffNorth, text: Cardiff North Cluster}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Organization-AmmanGwendraeth, text: Amman Gwendraeth Cluster}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Organization-NCMC, text: North Cardiff Medical Centre}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Organization-AmmanTawe, text: Amman Tawe Partnership}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Organization-MedicalInsurer, text:Example Organization - Medical Insurer}}</li>
    </list>
  </div>
</div>

### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Mandatory-and-Must-Support-Data-Elements,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.

Each Organisation must support:
* An identifier*
  * The `Organization.identifier` field **SHOULD** contain all available identifiers. In particular:
    * The [Organisation Data Service](https://digital.nhs.uk/services/organisation-data-service) (ODS) issues and manages unique identification codes and accompanying reference data for organisations that interact with any area of the NHS. The ODS code for organisations managed by this service **SHOULD** be populated (this includes ANANA format codes). 
    * The Welsh Reference and Terminology Service (WRTS) ensures that each organisation in the Welsh reference data has a unique code that **SHOULD** be populated. Where appropriate the codes issued by ODS or other national bodies are adopted. <br /><br />

* The active status of the organisation
  * The `Organization.active` field **SHOULD** be populated to indicate whether the organisation is still active.  <br /><br />

* Details of `Organization.type`, structured to comprise sector plus a hierarchical organisation type 
  * `sector` **SHOULD** be provided to distinguish public, private and third sector organisations
  * `domain` **SHOULD** be provided to identify the domain or industry in which the organisation operates
  * `classification` **SHOULD** be provided as a high level classification of the organisation type within the applicable domain.
  * `subclassification` **SHOULD** be provided as a lower level classification of the organisation type within the applicable domain.  <br /><br />

* `Organization.name` **SHOULD** be populated.
* For each `Organization.alias`, an `aliasType` extension **SHOULD** specify the nature of the alias.

* Where applicable:
  * the `Organization.partOf` field **SHOULD** contain a reference to the parent Organization
  * the `Organization.telecom` field **SHOULD** contain at least one contact point (e.g. telephone number)
  * the `Organization.address` field **SHOULD** contain at least one address for the organisation

_*See implementation guidance for the identifier element in the Slices section below_

### Extensions

The following extensions are defined for use within this profile: 
* Data Standards Wales Extensions:
    * {{pagelink:Extension-DataStandardsWales-AliasType}} is used to specify the nature of each alias.
    * {{pagelink:Extension-DataStandardsWales-SuccessorOrganization}} is used to identify the successor organisation that continues the delivery of services after the end date recorded for the organisation.
* UK Core Extensions:
    * [Extension-UKCore-AddressKey](https://simplifier.net/resolve?scope=package:fhir.r4.ukcore.stu2@2.0.1&filepath=package/Extension-UKCore-AddressKey.json) extends the Address datatype to support the storage of address identifiers such as the Unique Property Reference Number (UPRN).
    * [Extension-UKCore-MainLocation](https://simplifier.net/guide/uk-core-implementation-guide-stu2/Home/ProfilesandExtensions/ExtensionLibrary/Extension-UKCore-MainLocation?version=2.0.1) extends the Organization resource to support the exchange of information on the organisation's main location, as a reference to a Location resource.
* HL7 International Extensions:
    * [Organization-Period](http://hl7.org/fhir/R4/extension-organization-period.html) describes the date range that the organisation should be considered available.
    * [Translation](https://www.hl7.org/fhir/R4/extension-translation.html) supports Welsh named organisations.
  
### Slices

Slices apply to the following elements:
* `Organization.identifier` 
  * `Organization.identifier:wrtsOrganizationIdentifier`. See the description of Welsh Reference and Terminology Service (WRTS) identifiers under Mandatory and Must Support Data Elements above.
  * `Organization.identifier:odsOrganisationCode`. The ODS Organisation Code is further described here: [UK Core Naming System](https://simplifier.net/guide/UKNamingSystems/Home?version=current)
  * `Organization.identifier:gpClusterCode`. This slice was DEPRECATED at 2.6.0 and is marked as WITHDRAWN at 2.7.0. It applied to only a small proportion of organisations and was misnamed for its intended use. The identifier for a WRTS cluster can be recorded as a generic identifier using the WRTS cluster code namespace. It will also be represented in the wrtsOrganizationIdentifier slice.  <br /><br />

* `Organization.type` includes a slice for each of the four organisation type variants described above under Mandatory and Must Support Data Elements: 
  * `Organization.type:sector`
  * `Organization.type:domain`
  * `Organization.type:classification`
  * `Organization.type:subclassification` 

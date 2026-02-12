<div class="warning"><span class="ImplementWarn"></span></div>

## {{page-title}}

### Overview
The [Location](https://www.hl7.org/fhir/r4/location.html) resource contains information about a physical or virtual place where services are provided and resources and participants may be stored, found, contained, or accommodated. Typical examples include buildings, wards, corridors, rooms or beds, but may also include mobile clinics, a vehicle or lift, or a patient's home. 

The {{page-title}} profile is derived from the [UK Core Location Profile](https://simplifier.net/guide/uk-core-implementation-guide-stu2/Home/ProfilesandExtensions/Profile-UKCore-Location?version=2.0.1). It defines additional rules for use within health and care organisations in Wales. Further guidance on the use of the Location resource along with other administrative FHIR resources is provided within the {{pagelink:Home/Guidance/Administrative-Data, text: guidance}} section of this guide.

A direct link to the Data Standards Wales asset can be accessed here - {{link:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Location}}

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Location, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Location, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Location, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>{{pagelink:Example-DataStandardsWales-Location-CadogWard, text:Example Location - Cadog Ward (GGH)}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Location-WardE, text:Example Location - Ward E (NPT)}}</li>
    </list>
  </div>    
</div>

### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Mandatory-and-Must-Support-Data-Elements,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.
 
Each Location must have:
* A name
  * The `Location.name` field **SHALL** be populated.

Each Location must support:
* An identifier*
  * The `Location.identifier` field **SHOULD** contain all available identifiers. Typical identifiers include:
    * Identifiers assigned to the location by the Welsh Reference Data Service
    * Other identifiers assigned by a hospital PAS or other clinical system.  <br /><br />

* A status of the location (i.e. whether it is active, suspended or inactive)
  *  The `Location.status` field **SHOULD** be populated to indicate whether the organization is active, suspended or inactive.  <br /><br />

* Details of `Location.type`, ideally structured to comprise a hierarchical location type appropriate to the domain of the managing organization:
  * `classification` **SHOULD** be provided as a high level classification of the location type.
  * `subclassification` **SHOULD** be provided as a lower level classification of the location type.  <br /><br />

* For each `Location.alias`, an `aliasType` extension **SHOULD** specify the nature of the alias.

* Where applicable:
  * the `Location.partOf` field **SHOULD** contain a reference to the location that this location is physically part of.
  * the `Location.managingOrganization` field **SHOULD** contain a reference to the organization that manages the service delivery at the location.
  * the `Location.address` field **SHOULD** contain at least one address for the location.

_*See implementation guidance for the identifier element in the Slices section below_

### Extensions

The following extensions are defined for use within this profile: 
* The UK Core extension [Extension-UKCore-AddressKey](https://simplifier.net/resolve?scope=package:fhir.r4.ukcore.stu2@2.0.1&filepath=package/Extension-UKCore-AddressKey.json) extends the Address datatype to support the storage of additional address identifiers.

* {{pagelink:Extension-DataStandardsWales-AliasType}} is used to specify the nature of each alias.
* {{pagelink:Extension-DataStandardsWales-GridReference}} is used to specify the northings and eastings applicable to the location.
* {{pagelink:Extension-DataStandardsWales-LocationPeriod}} is used to specify fixed characteristics of the location such as wheelchair access.
* {{pagelink:Extension-DataStandardsWales-LocationPeriod}} is used to specify the active period for the location.

### Slices

Slices apply to the following elements:
* `Location.identifier`.  The namespaces denoting issuing authority for the identifier are defined on the {{pagelink:Naming-Systems, text:Naming Systems}} page.  A dedicated slice is provided for the WRTS location identifier:
  * `Location.identifier:wrtsLocationIdentifier`. <br /><br />

* `Location.type` includes a slice for each of the two type variants described above under Mandatory and Must Support Data Elements: 
  * `Location.type:classification`
  * `Location.type:subclassification` 

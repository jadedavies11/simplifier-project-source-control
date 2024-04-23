<div class="warning"><span class="ImplementWarn"></span></div>

## {{page-title}}

### Overview
The [Location](https://hl7.org/fhir/location.html) resource contains information about a physical place where services are provided and resources and participants may be stored, found, contained, or accommodated. Typical examples include buildings, wards, corridors, rooms or beds, but may also include mobile clinics, a vehicle or lift, or a patient's home. 

The {{page-title}} profile is derived from the [UK Core Location Profile](https://simplifier.net/guide/uk-core-implementation-guide/Home/ProfilesandExtensions/ProfileUKCore-Location?version=1.0.0). It defines additional rules for use within health and care organisations in Wales. Further guidance on the use of the Location resource along with other administrative FHIR resources is provided within the {{pagelink:Home/Guidance/Administrative-Data, text: guidance}} section of this guide.

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
When an element is mandatory (min=1), the data is expected to always be present. Elements marked with an <span style="background-color:red;color:white;">S</span> must be supported by both producing and receiving systems and **SHOULD** be populated if the data exists.
 
Each Location must have:
1. A name

Each Location must support:
1. An identifier *
2. A status of the location (i.e., whether it is active, suspended or inactive)

*see Implementation Guidance for the identifier element below


The `Location.identifier` field **SHOULD** contain all available identifiers. Typical identifiers include:
  * Identifiers assigned to the location by the Welsh Reference Data Service
  * Other identifiers assigned by a hospital PAS or other clinical system.

The `Location.status` field **SHOULD** be populated to indicate whether the organization is active, suspended or inactive.

The `Location.name` field **SHALL** be populated.

### Slices
The following identifier slice is used with the location profile listed below. The namespaces denoting issuing authority for the identifier are defined on the {{pagelink:Home/FHIR-Assets/Naming-Systems.page.md, text:Naming Systems}} page.
 
* `Location.identifier:wrtsLocationIdentifier` 



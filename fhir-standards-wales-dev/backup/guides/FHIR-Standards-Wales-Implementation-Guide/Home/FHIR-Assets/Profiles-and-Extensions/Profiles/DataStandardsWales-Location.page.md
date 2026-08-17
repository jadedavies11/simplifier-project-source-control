## {{page-title}}

### Overview
The [Location](https://www.hl7.org/fhir/r4/location.html) resource contains information about a physical place where services are provided and resources and participants may be stored, found, contained, or accommodated. Typical examples include buildings, wards, corridors, rooms or beds, but may also include mobile clinics, a vehicle or lift, or a patient's home. 

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
      <li>{{pagelink:Example-DataStandardsWales-Location-AmmanTawePartnership, text:Example Location - Amman Tawe Partnership GP Surgery}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Location-BrynammanCommunity, text:Example Location - Brynamman Community GP Surgery}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Location-CadogWard, text:Example Location - Cadog Ward (GGH)}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Location-GGH, text:Example Location - Glangwili General Hospital}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Location-MeddygfaCwmamman, text:Example Location - Meddygfa Cwmamman GP Surgery}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Location-GGH-OPD, text:Example Location - Outpatients Department (GGH)}}</li>
      <li>{{pagelink:Example-DataStandardsWales-Location-WardE, text:Example Location - Ward E (NPT)}}</li>
    </list>
  </div>    
</div>

### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Mandatory-and-Must-Support-Data-Elements,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.
 
Each Location must support:
1. An identifier *
2. A status of the location (i.e. whether it is active, suspended or inactive)
3. A name of the location
4. An address for the location
5. A physical form of the location
6. A managing organization for the location
7. A part of reference to signify if a location is physically part of another location

*see Implementation Guidance for the identifier element below

The `Location.identifier` field **SHOULD** contain all available identifiers. Typical identifiers include:
  * Identifiers assigned to the location by the Welsh Reference Data Service
  * Other identifiers assigned by a hospital PAS or other clinical system.

The `Location.status` field **SHOULD** be populated to indicate whether the organization is active, suspended or inactive.


### Slices
The following identifier slice is used with the location profile listed below. The namespaces denoting issuing authority for the identifier are defined on the {{pagelink:Home/FHIR-Assets/Naming-Systems}} page.
 
* `Location.identifier:wrtsLocationIdentifier` 
* `Location.identifier:glnCode` 
* `Location.identifier:gphcPremisesNumber` 
* `Location.identifier:nwsspPharmacyAccountNumber` 
* `Location.identifier:nhsbsaOpticianContractNumber` 
* `Location.identifier:nhsbsaDentalLocationIdentifier` 

### Extensions
The extensions listed below allow a number of the data elements listed above to be supported where not currently supported by the Data Standards Wales Location profile:
* Data Standards Wales Extensions:
    * {{pagelink:Extension-DataStandardsWales-LocationPeriod}} supports the date range that this location should be considered available.
    * {{pagelink:Extension-DataStandardsWales-GridReference}} supports recording the national grid reference applicable to the location.
* HL7 International Extensions:
    * [Translation](https://www.hl7.org/fhir/R4/extension-translation.html) supports Welsh named locations.
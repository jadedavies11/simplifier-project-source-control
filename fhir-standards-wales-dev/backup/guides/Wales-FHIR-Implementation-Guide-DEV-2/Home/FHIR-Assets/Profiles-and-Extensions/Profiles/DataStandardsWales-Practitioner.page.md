<div class="warning"><span class="ImplementWarn"></span></div>

## {{page-title}}

### Overview
The [Practitioner](https://hl7.org/fhir/practitioner.html) resource defines an individual member of a clinical profession with responsibility for delivering care within the health system. 

The {{page-title}} 
profile is derived from the [UK Core Practitioner Profile](https://simplifier.net/guide/uk-core-implementation-guide/Home/ProfilesandExtensions/Profile-UKCore-Practitioner?version=1.0.0). It defines additional rules for use within health and care organisations in Wales. 

Further guidance on the use of the Practitioner resource along with other administrative FHIR resources is provided within the {{pagelink:Home/Guidance/Administrative-Data, text: guidance}} section of this guide.

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Practitioner, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Practitioner, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Practitioner, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>{{pagelink:Example-DataStandardsWales-Practitioner-Consultant, text:Example Practitioner - Dhiren Patel (Consultant) }}</li>
      <li>{{pagelink:Example-DataStandardsWales-Practitioner-Physiotherapist, text:Example Practitioner - Philip Wickins (Physiotherapist) }}</li>
      <li>{{pagelink:Example-DataStandardsWales-Practitioner-PrescribingNurse, text:Example Practitioner - Sandra Huggins (Prescribing Nurse) }}</li>
    </list>
  </div>
</div>

### Mandatory and Must Support Data Elements
When an element is mandatory (min=1), the data is expected to always be present. Elements marked with an <span style="background-color:red;color:white;">S</span> must be supported by both producing and receiving systems and **SHOULD** be populated if the data exists.

Each Practitioner record must have:
1. A `Practitioner.name` to indicate the name by which the individual is known.

Each Practitioner record must support:
1. A `Practitioner.identifier` to indicate the unique identifier(s) under which the individual is registered.

### Slices
The following slices are defined for use within this profile. The namespaces denoting issuing authority for each identifier are defined by HL7 UK with the exception of `Practitioner.identifier:nadexIdentifier` which is defined on the {{pagelink:Home/FHIR-Assets/Naming-Systems.page.md, text:NHS Wales Naming Systems}} page.
* `Practitioner.identifier`
* `Practitioner.identifier:gdcNumber`
* `Practitioner.identifier:gmcNumber`
* `Practitioner.identifier:gmpNumber`
* `Practitioner.identifier:hcpcNumber`
* `Practitioner.identifier:nmcNumber`
* `Practitioner.identifier:gphcCode`
* `Practitioner.identifier:sdsUserId`
* `Practitioner.identifier:nadexIdentifier`





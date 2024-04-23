<div class="warning"><span class="ExperiWarn"></span></div>

## {{page-title}}
The [Immunization](https://hl7.org/fhir/immunization.html) resource is a record of the immunization received by a patient.

The {{page-title}} profile is derived from the [UK Core Immunization Profile](https://simplifier.net/guide/uk-core-implementation-guide/Home/ProfilesandExtensions/ProfileUKCore-Immunization?version=1.0.0). It defines additional rules for use within health and care organisations in Wales.

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Immunization, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Immunization, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Immunization, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>Currently under development</li> 
    </list>
  </div>    
</div>

### Mandatory and Must Support Data Elements
When an element is mandatory (min=1), the data is expected to always be present. Elements marked with an <span style="background-color:red;color:white;">S</span> must be supported by both producing and receiving systems and **SHOULD** be populated if the data exists.

Each Immunization must have:
1. status
2. vaccineCode
3. patient
4. occurance

Each Immunization must support:
1. identifier
2. statusReason
3. recorded
4. reportOrigin
5. location
6. manufacturer
7. lotNumber
8. expirationDate
9. site
10. route
11. doseQuantity
12. performer
13. reasonCode
14. protocolApplied
<div class="warning"><span class="ImplementWarn"></span></div>

## {{page-title}}
The [MedicationAdministration](https://hl7.org/fhir/medicationadministration.html) resource is a record of a medication that is administered to a patient.

The {{page-title}} profile is derived from the [UK Core MedicationAdministration Profile](https://simplifier.net/guide/uk-core-implementation-guide/Home/ProfilesandExtensions/ProfileUKCore-MedicationAdministration?version=1.0.0). It defines additional rules for use within health and care organisations in Wales.

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-MedicationAdministration, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-MedicationAdministration, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-MedicationAdministration, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>Currently under development</li> 
    </list>
  </div>    
</div>

### Mandatory and Must Support Data Elements
When an element is mandatory (min=1), the data is expected to always be present. Elements marked with an <span style="background-color:red;color:white;">S</span> must be supported by both producing and receiving systems and **SHOULD** be populated if the data exists.
 
Each MedicationAdministration must have:
1. status
2. medication
3. subject
4. effective
5. performer

Each MedicationAdministration must support:
1. identifier
2. statusReason
3. request
4. dosage
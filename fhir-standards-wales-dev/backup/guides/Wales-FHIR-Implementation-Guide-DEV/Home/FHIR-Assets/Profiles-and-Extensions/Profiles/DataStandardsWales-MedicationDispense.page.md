<div class="warning"><span class="ImplementWarn"></span></div>

## {{page-title}}
The [MedicationDispense](https://hl7.org/fhir/medicationdispense.html) resource is a record of a medication that is dispensed to a patient.

The {{page-title}} profile is derived from the [UK Core MedicationDispense Profile](https://simplifier.net/guide/uk-core-implementation-guide/Home/ProfilesandExtensions/ProfileUKCore-MedicationDispense?version=1.0.0). It defines additional rules for use within health and care organisations in Wales.

For additional guidance on implementation of UK Core, [see here](https://simplifier.net/guide/UK-Core-Implementation-Guide/Home?version=1.0.0).

A direct link to the Data Standards Wales asset can be accessed here - {{link:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-MedicationDispense}}

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-MedicationDispense, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-MedicationDispense, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-MedicationDispense, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>Currently under development</li> 
    </list>
  </div>    
</div>

### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Home/Introduction/Profile-Descriptions/Mandatory-and-Must-Support-Data-Elements.page.md,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.
 
Each MedicationDispense must have:
1. status
2. medication

Each MedicationDispense must support:
1. identifier
2. statusReason
3. subject
4. performer
5. authorizingPrescription
6. type
7. quantity
8. daysSupply
9. whenPrepared
10. whenHandedOver
11. dosageInstructions
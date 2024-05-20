<div class="warning"><span class="ExperiWarn"></span></div>

## {{page-title}}

### Overview
The [Provenance](https://www.hl7.org/fhir/r4/provenance.html) resource tracks information about the activity that created, revised, deleted, or signed a version of a resource, describing the entities and agents involved.

The {{page-title}} profile is derived from the [HL7 FHIR UK Core R4](https://fhir.hl7.org.uk/StructureDefinition/UKCore-Provenance) and is therefore listed as experimental. It defines additional rules for use within health and care organisations in Wales. (add note that UK Core profile is a draft and under development)

A direct link to the Data Standards Wales asset can be accessed here - {{link:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Provenance}}


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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Provenance, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Provenance, diff}}
	</div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Provenance, hybrid}}
	</div>
  <div id="tabeg" class="tabcontent">
  </div>
</div>

### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Home/Introduction/Profile-Descriptions/Mandatory-and-Must-Support-Data-Elements.page.md,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.
 
**Each Provenance must have:**
1. The instant of time at which the activity was recorded
1. The individual, device or organization that participated in the event
1. How the entity was used during the activity
1. Identity of entity
1. When the digital signature was signed
1. Who signed

**Each Provenance must support:**
1. Target Reference
1. The instant of time at which the activity was recorded
1. Actor involved
1. A digital signature on the target Reference

### Implementation Guidance (do we require this?)
* The `Provenance.agent.who` field **SHALL** be populated.
* The `Specimen.subject` reference field **SHALL** be populated.
<br><br>


### Extension (do i list all the extension elements in DemographicsAsRecorded?)
The extension listed below has been created to support PAS entries: 

* [NHS Wales-DemographicsAsRecorded](https://simplifier.net/guide/Wales-FHIR-Implementation-Guide-v1.1.0/Home/FHIR-Assets/Profiles-and-Extensions/Extensions/Extension-DataStandardsWales-DemographicsAsRecorded.page.md?version=current) extends the Provenance resource to capture demographics details recorded as at the time of the care record change
         

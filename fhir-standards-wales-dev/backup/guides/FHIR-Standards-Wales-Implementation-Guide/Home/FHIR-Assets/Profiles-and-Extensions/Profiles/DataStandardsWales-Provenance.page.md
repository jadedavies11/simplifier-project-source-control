<div class="warning"><span class="ExperiWarn"></span></div>

## {{page-title}}

### Overview
The [Provenance](https://www.hl7.org/fhir/r4/provenance.html) resource tracks information about the activity that created, revised, deleted, or signed a version of a resource, describing the entities and agents involved.

The {{page-title}} profile is derived from the [HL7 R4 Provenance](http://hl7.org/fhir/Provenance.html). It defines additional rules for use within health and care organisations in Wales.

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
    <list>
        <li>{{pagelink:Example-DataStandardsWales-Provenance-Amend, text:Example Provenance - Patient demographic update as result of an HL7v2 update }}</li>
        <li>{{pagelink:Example-DataStandardsWales-Provenance-Growth-Charts, text:Example Provenance - Provenance record with multiple targets }}</li>
        <li>Example Provenance - Recording demographic as recorded (TODO) Link also to be provided from the Extension's definition page</li>
      </list>
  </div>
</div>

### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Home/Introduction/Profile-Descriptions/Mandatory-and-Must-Support-Data-Elements.page.md,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.
 
Each Provenance must have:
1. One or more targets
1. A recorded timestamp

Each Provenance must support:
1. One or more agents
1. One or more entities if relevant

### Implementation Guidance 
The `Provenance.target` field **SHALL** be populated to reference the FHIR resource(s) that were generated or updated by the activity described in this resource. A provenance can point to more than one target if multiple resources were created/updated by the same activity.

The `Provenance.recorded` field **SHALL** be include a timestamp to indicate when the activity was recorded/updated.

The `Provenance.agent` field **SHOULD** include all agents involved in the activity. Typical agents include
* Devices such as software systems or components
* Clinical devices 
* Human users

The `Provenance.entity` field **MAY** be used to indicate one or more entities in this activity, and may be used to refer, for example, to an HL7v2 message used to update demographic information within a Patient resource. 

Please see the Provenance page within the Guidance section above for further information. 

### Extensions 
Some use cases require the original demographic data at time of recording to stored directly against the clinical data e.g. for diagnostic reports in Wales. This additional provenace can be captured using the {{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Extensions/Extension-DataStandardsWales-DemographicsAsRecorded.page.md,text:DataStandardsWales-DemographicsAsRecorded}} extension.
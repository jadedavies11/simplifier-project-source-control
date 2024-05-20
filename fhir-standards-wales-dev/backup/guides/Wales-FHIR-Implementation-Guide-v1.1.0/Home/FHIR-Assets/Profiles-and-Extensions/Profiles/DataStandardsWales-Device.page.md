<div class="warning"><span class="ExperiWarn"></span></div>

## {{page-title}}
The [Device](https://www.hl7.org/fhir/r4/device.html) profile captures the type of a manufactured item that is used in the provision of healthcare without being substantially changed through that activity. The device may be a medical or non-medical device.

The {{page-title}} profile is derived from the [HL7 FHIR UK Core R4](https://fhir.hl7.org.uk/StructureDefinition/UKCore-Device) and is therefore listed as experimental. It defines additional rules for use within health and care organisations in Wales. (add note that UK Core profile is a draft and under development)

A direct link to the Data Standards Wales asset can be accessed here - {{link:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Device}}

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Device, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Device, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Device, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
  </div>
</div>



### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Home/Introduction/Profile-Descriptions/Mandatory-and-Must-Support-Data-Elements.page.md,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.
 
**Each Device must have:**
1. The name of the device
1. The type of deviceName
1. The standard that is used to operate and communicate
1. The version text
1. Code that specifies the property DeviceDefinitionPropetyCode
1. Who signed

**Each Device must support:**

1. 

### Implementation Guidance (do we require this?)
* 



### Slice
The following identifier slice is to be used with the device profile is listed below. 
 
* `Device.identifier:applicationInstanceId` 

         

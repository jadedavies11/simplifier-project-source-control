<div class="warning"><span class="ExperiWarn"></span></div>

## {{page-title}}
The [Dosage](https://www.hl7.org/fhir/r4/dosage.html) resource is a record of a medication that is administered to a patient.

The {{page-title}} profile is derived from the [HL7 Dosage Profile](https://www.hl7.org/fhir/r4/dosage.html). It defines additional rules for use within health and care organisations in Wales.

A direct link to the Data Standards Wales asset can be accessed here - {{link:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Dosage}}

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Dosage, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Dosage, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Dosage, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>Currently under development</li> 
    </list>
  </div>    
</div>

#### Example Usage Scenarios
The {{page-title}} will unlikely be used in isolation and will tipically used as a referenced resource within
<div class="tab-wrap">
  <ul class="tab-head">
  <div id="tabeg" class="tabcontent">
    <list>
      <li>{{pagelink: Home/FHIR-Assets/Profiles-and-Extensions/Profiles/DataStandardsWales-Medication.page.md}}</li>
      <li>{{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/DataStandardsWales-MedicationAdministration.page.md}}</li>
      <li>{{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/DataStandardsWales-MedicationDispense.page.md}}</li>
      <li>{{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/DataStandardsWales-MedicationList.page.md}}</li>
      <li>{{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/DataStandardsWales-MedicationRequest.page.md}}</li>
      <li>{{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/DataStandardsWales-MedicationStatement.page.md}}</li>
    </list>
  </div>
  </ul>
</div>

### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Home/Introduction/Profile-Descriptions/Mandatory-and-Must-Support-Data-Elements.page.md,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.

Each Dosage must support:

|Element|Reason|
|-|-|
|`sequence`|Multi-sequence dosage instructions.|
|`text`|The complete dosage instruction as a human readable string.|
|`additionalInstruction`|Additional dosage instructions that can be either SNOMED-CT coded terms or free-text instructions.|
|`patientInstruction`|Patient or consumer oriented instructions.|
|`timing`|When medication should be administered.|
|`asNeeded`|Take "as needed" (for x).|
|`site`|Body site to administer to.|
|`route`|How drug should enter body.|
|`method`|Technique for administering medication.|
|`maxDosePerPeriod`|Upper limit on medication per unit of time.|

### Bindings (differential)
More information about the bindings can be found below

|Context|Strength|Link|
|-|-|-|
|Dosage.additionalInstruction|example|[SNOMEDCT-AdditionalDosageInstructions](https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Dosage)|
|Dosage.timing.repeat.durationUnit|required|[Units of Time](https://simplifier.net/resolve?scope=hl7.fhir.r4.core@4.0.1&filepath=package/ValueSet-units-of-time.json)|



<div class="warning"><span class="ImplementWarn"></span></div>

## {{page-title}}

### Overview
The [List](https://hl7.org/fhir/list.html) resource is a curated collection of resources. The Allergy List profile is intended to provide a snapshot view of a patient's allergies.

The {{page-title}} profile is derived from the [UK Core List Profile](https://simplifier.net/packages/fhir.r4.ukcore.stu1/1.0.0/files/806176). It defines additional rules for use within health and care organisations in Wales.

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-AllergyList, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-AllergyList, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-AllergyList, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>{{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/Examples/Allergies/Example-DataStandardsWales-List-Allergies.page.md, text:Example List - with Allergies}}</li>  
            <li>{{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/Examples/Allergies/Example-DataStandardsWales-List-Allergies-Empty.page.md, text:Example List - empty list}}</li>  
                  <li>{{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/Examples/Allergies/Example-DataStandardsWales-List-Allergies-NoKnownAllergy.page.md, text:Example List - with no known Allergies}}</li>    
    </list>
  </div>    
</div>

### Mandatory and Must Support Data Elements
When an element is mandatory (min=1), the data is expected to always be present. Elements marked with an <span style="background-color:red;color:white;">S</span> must be supported by both producing and receiving systems and **SHOULD** be populated if the data exists.
 
Each Allergy List must have:
1. A status
2. A mode
3. A fixed SNOMED CT code of value of 886921000000105|'Allergies and adverse reactions'
4. A subject (patient)


Each Allergy list must support:
1. An encounter
2. A source to indicate who defined the list contents


The mode is always expected to indicate the list represents a snapshot of an allergy information that is potentially derived from another source.
<br><br>
The `List.code` field **SHALL** be SNOMED CT coded to 'allergies and adverse reactions'.
<br><br>
The resource **SHALL** include a reference to the subject (patient).




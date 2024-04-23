<div class="warning"><span class="ImplementWarn"></span></div>

## {{page-title}}

### Overview

The [PractitionerRole](https://hl7.org/fhir/practitionerrole.html) resource defines the role of a clinical profession with responsibility for delivering care within the health system. 

The {{page-title}} profile is derived from the [UK Core PractitionerRole Profile](https://simplifier.net/guide/uk-core-implementation-guide/Home/ProfilesandExtensions/ProfileUKCore-PractitionerRole?version=1.0.0). It defines additional rules for use within health and care organisations in Wales. 

Further guidance on the use of the PractitionerRole resource along with other administrative FHIR resources is provided within the {{pagelink:Home/Guidance/Administrative-Data, text: guidance}} section of this guide. 

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-PractitionerRole, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-PractitionerRole, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-PractitionerRole, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>{{pagelink:Example-DataStandardsWales-PractitionerRole-Consultant, text:Example PractitionerRole - Consultant (Geriatric Medicine) }}</li>
      <li>{{pagelink:Example-DataStandardsWales-PractitionerRole-Physiotherapist, text:Example PractitionerRole - Physiotherapist }}</li>
      <li>{{pagelink:Example-DataStandardsWales-PractitionerRole-PrescribingNurse, text:Example PractitionerRole - Prescribing Nurse }}</li>
    </list>
  </div>   
</div>

### Mandatory and Must Support Data Elements
When an element is mandatory (min=1), the data is expected to always be present. Elements marked with an <span style="background-color:red;color:white;">S</span> must be supported by both producing and receiving systems and **SHOULD** be populated if the data exists.

Each PractitionerRole must have:
1. A code to indicate job role

Each PractitionerRole must support:
1. An indicator that the role is still active
2. The period that the role was active
3. A link to the practitioner who is performing the role
4. A link to the organisation where the role is performed
5. The practitioner's specialty in the role



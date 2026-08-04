## {{page-title}}

### Overview

The [OrganizationAffiliation](https://www.hl7.org/fhir/R4/organizationaffiliation.html) resource contains information the relationship between two organizations over a period of time, where the entities are separate business entities. The relationship can optionally include details of locations/services from the participating organization.


A direct link to the Data Standards Wales asset can be accessed here - {{link:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-OrganizationAffiliation}}

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-OrganizationAffiliation, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-OrganizationAffiliation, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-OrganizationAffiliation, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>Currently under development</li>
    </list>
  </div>
</div>

### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Mandatory-and-Must-Support-Data-Elements,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.

Each OrganisationAffiliation must have:
* An Organization
  * The `OrganizationAffiliation.organization` field **SHALL** be populated.

Each Organisation must support:
* An identifier*
  * `OrganizationAffiliation.wrtsAffiliationIdentifier` 
  * `OrganizationAffiliation.participatingOrganization`
  * `OrganizationAffiliation.code`  
  * `OrganizationAffiliation.location` <br /><br />

  
### Slices

Slices apply to the following elements:
* `OrganizationAffiliation.identifier` 
  * `Organization.identifier:wrtsAffiliationIdentifier`<br /><br />



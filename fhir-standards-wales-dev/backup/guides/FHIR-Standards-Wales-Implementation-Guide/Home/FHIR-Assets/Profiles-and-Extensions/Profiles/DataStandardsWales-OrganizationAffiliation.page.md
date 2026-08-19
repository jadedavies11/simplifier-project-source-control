## {{page-title}}

### Overview

The [OrganizationAffiliation](https://www.hl7.org/fhir/R4/organizationaffiliation.html) resource supports formal and enduring one-to-many and many-to-many relationships between organisations, that fall outside of the strict organisation hierarchy. Each OrganizationAffiliation resource links a pair of organisations. One organisation can be considered to own the arrangement, while the other is a participating organisation. The relationship can optionally include details of the involved locations and healthcare services of the participating organisation.

The DataStandardsWales-OrganizationAffiliation profile is derived from the [HL7 R4 OrganizationAffiliation](https://www.hl7.org/fhir/R4/organizationaffiliation.html) resource. It defines additional rules for use within health and care organisations in Wales.

For example, within NHS Wales a "region" organisation represents a set of health board organisations that collaborate to provide certain services for their joint populations. This arrangement can be instantiated as a series of OrganizationAffiliation resources, each associating the owning region with a participating health board.

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
      <li>{{pagelink:Example-DSW-OrganizationAffiliation-CC201-W00142, text:Example Cluster Affiliation - Amman Gwendraeth and Amman Tawe Partnership}}</li>
    </list>
  </div>
</div>

### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Mandatory-and-Must-Support-Data-Elements,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.

Each OrganisationAffiliation must have:
* An Organization
  * The `OrganizationAffiliation.organization` field **SHALL** be populated.

Each Organisation must support:
* An identifier: `OrganizationAffiliation.wrtsAffiliationIdentifier` field SHOULD be populated
* A participating organisation: `OrganizationAffiliation.participatingOrganization` field SHOULD be populated
* An affiliation type: `OrganizationAffiliation.code` field SHOULD be populated  
* One or more locations, if applicable: `OrganizationAffiliation.location`  field SHOULD be populated where applicable to the relationship <br /><br />

  
### Slices

Slices apply to the following elements:
* `OrganizationAffiliation.identifier` 
  * `Organization.identifier:wrtsAffiliationIdentifier`<br /><br />



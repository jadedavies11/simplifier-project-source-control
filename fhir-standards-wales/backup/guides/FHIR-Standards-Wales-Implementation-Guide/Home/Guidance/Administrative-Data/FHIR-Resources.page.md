## {{page-title}}
The involved FHIR resources are described in the tabs below. For each, the relationships with the other administrative data resources listed above are illustrated, together with potential scenarios for use in the clinicial record. 

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openLocalTab(this,'tabresorganization')" data-target="tabresorganization">
      Organization
    </li>
    <li class="tablink" onclick="openLocalTab(this,'tabreslocation')" data-target="tabreslocation">
      Location
    </li>   
    <li class="tablink" onclick="openLocalTab(this,'tabresservice')" data-target="tabresservice">
      HealthcareService
    </li>  
    <li class="tablink" onclick="openLocalTab(this,'tabresaffiliation')" data-target="tabresaffiliation">
      OrganizationAffiliation
    </li>
	  <li class="tablink" onclick="openLocalTab(this,'tabrespractitioner')" data-target="tabrespractitioner">
      Practitioner
    </li> 
	  <li class="tablink" onclick="openLocalTab(this,'tabresrole')" data-target="tabresrole">
      PractitionerRole
    </li>  
  </ul>
  <div class="tab-main">
    <div id="tabresorganization" class="tabcontent active">
       {{page:RES-Organization}}
    </div>
	  <div id="tabreslocation" class="tabcontent">
       {{page:RES-Location}}
    </div>
	  <div id="tabresservice" class="tabcontent">
       {{page:RES-HealthcareService}}
    </div>
	  <div id="tabresaffiliation" class="tabcontent">
       {{page:RES-OrganizationAffiliation}}
    </div>
	  <div id="tabrespractitioner" class="tabcontent">
       {{page:RES-Practitioner}}
    </div>
	  <div id="tabresrole" class="tabcontent">
       {{page:RES-PractitionerRole}}
    </div>
  </div>
</div>
<br />
<br />
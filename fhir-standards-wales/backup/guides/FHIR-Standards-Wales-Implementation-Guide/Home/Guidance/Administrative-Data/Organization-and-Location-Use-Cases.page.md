## {{page-title}}
The {{pagelink:DataStandardsWales-Organization, text: Organization}} resource supports a formal decomposition hierarchy via a `partOf` link to the parent organization.  In the case of {{pagelink:DataStandardsWales-Location, text: Location}} the `partOf` link describes a physical decomposition e.g. a room is part of the building it sits within.  The two hierarchies are linked by the identification of the `managingOrganization` for each Location, and by use of the `mainLocation` extension on the Organization resource. The structural hierarchies are illustrated in the Secondary Care Hierarchies and General Practice Hierarchies use cases below.

For any organizational relationships that sit outside of the formal structural hierarchy, the {{pagelink:DataStandardsWales-OrganizationAffiliation, text: OrganizationAffiliation}} resource is used.  The two main use cases in Wales are covered by the Primary Care Clusters and Healthcare Regions tabs.

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openLocalTab(this,'tabusesecondary')" data-target="tabusesecondary">
      Secondary Care Hierarchies
    </li>
    <li class="tablink" onclick="openLocalTab(this,'tabusegp')" data-target="tabusegp">
      General Practice Hierarchies
    </li>   
    <li class="tablink" onclick="openLocalTab(this,'tabusecluster')" data-target="tabusecluster">
      Primary Care Clusters
    </li>  
    <li class="tablink" onclick="openLocalTab(this,'tabuseregion')" data-target="tabuseregion">
      Healthcare Regions
    </li>
  </ul>
  <div class="tab-main">
    <div id="tabusesecondary" class="tabcontent active">
       {{page:USE-Secondary-Care}}
    </div>
	<div id="tabusegp" class="tabcontent">
       {{page:USE-General-Practice}}
    </div>
	<div id="tabusecluster" class="tabcontent">
       {{page:USE-Primary-Care-Clusters}}
    </div>
	<div id="tabuseregion" class="tabcontent">
       {{page:USE-Healthcare-Regions}}
    </div>
  </div>
</div>
<br />
<br />
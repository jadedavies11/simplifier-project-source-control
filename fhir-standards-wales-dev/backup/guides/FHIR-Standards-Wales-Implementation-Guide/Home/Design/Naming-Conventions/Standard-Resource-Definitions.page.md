### {{page-title}}

See Glossary tab below for definitions of the components used throughout the naming standards​

The naming conventions for resource definitions in the Wales FHIR Implementation Guide are drawn up to be consistent across resource types.  The foundation of the naming convention is the filename, which is structured as <b><span style="color:#0070c0;">[Discriminator]-</span>DataStandardsWales-<span style="color:#c00000;">[BusinessName]</span></b>.xml

The filename is transformed as follows to provide the related elements in the resource definition and the filename.  In order to closely follow existing practice in UK and international implementation guides, there is some conditional treatment of the discriminator element.

<table class="table table-striped">
	<thead>
		<tr>
			<th scope="col"><b>Element</b></th>
			<th scope="col"><b>Construction</b></th>
			<th scope="col"><b>Rules</b></th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td scope="row">id</td>
			<td><b><span style="color:#0070c0;">{[Discriminator]-}</span>DataStandardsWales-<span style="color:#c00000;">[BusinessName]</span></b></td>
			<td>Same as filename, but discriminator omitted if it is “Profile”, or if it is the same as the HL7 level 2 resource type as in “CodeSystem”.</td>
		</tr>		
        <tr>
			<td scope="row">name</td>
			<td><b><span style="color:#0070c0;">{[Discriminator]}</span>DataStandardsWales<span style="color:#c00000;">[BusinessName]</span></b></td>
			<td>Based on id, with all hyphens removed.</td>
		</tr>	
        <tr>
			<td scope="row">title</td>
			<td><b><span style="color:#0070c0;">{[Discriminator]}</span> DataStandardsWales<span style="color:#c00000;"> [BusinessName]</span></b></td>
			<td>Based on id, with spaces between all words.</td>
        </tr>		
        <tr>
			<td scope="row">url</td>
			<td><b>[baseUrl]/<span style="color:#ff9900;">[L2ResourceType]/</span>[id]</b></td>
			<td>The id is referenced without amendment.</td>
        </tr>	
        <tr>
			<td scope="row"><i>reference</i></td>
			<td><b><span style="color:#ff9900;">[L2ResourceType]/</span>[id]</b></td>
			<td><i>Derived</i>. The resource definition can be uniquely referenced within the implementation guide omitting the base url.</td>
        </tr>	
    </tbody>
</table>

The filename and elements defined above are then reused in the definition of implementation guide pages:

<table class="table table-striped">
	<thead>
		<tr>
			<th scope="col"><b>Element</b></th>
			<th scope="col"><b>Construction</b></th>
			<th scope="col"><b>Rules</b></th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td scope="row">filename</td>
			<td><b><span style="color:#0070c0;">{[Discriminator]-}</span>DataStandardsWales-<span style="color:#c00000;">[BusinessName]</span></b>.page.md</td>
			<td>The same as xml asset filename.</td>
            </tr>	
    </tbody>
</table>

The specific application of this standard approach to resource definitions for each asset type is elaborated, with examples, in the tabs below.  In each case Discriminator and BusinessName are specialised as applicable to the asset type.​

The conventions for resources that diverge from this approach are described in dedicated sections.

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openLocalTab(this,'tabsrdglossary')" data-target="tabsrdglossary">
      Glossary
    </li>
    <li class="tablink" onclick="openLocalTab(this,'tabsrdprofile')" data-target="tabsrdprofile">
      Profile
    </li>
    <li class="tablink" onclick="openLocalTab(this,'tabsrdextension')" data-target="tabsrdextension">
      Extension
    </li>   
    <li class="tablink" onclick="openLocalTab(this,'tabsrdmsgdefinition')" data-target="tabsrdmsgdefinition">
      Message Definition
    </li>  
    <li class="tablink" onclick="openLocalTab(this,'tabsrdcodesystem')" data-target="tabsrdcodesystem">
      Code System
    </li>
	<li class="tablink" onclick="openLocalTab(this,'tabsrdvalueset')" data-target="tabsrdvalueset">
      Value Set
    </li>  
  </ul>
  <div class="tab-main">
    <div id="tabsrdglossary" class="tabcontent">
       {{page:SRD-Glossary}}
    </div>
    <div id="tabsrdprofile" class="tabcontent">
       {{page:SRD-Profile}}
    </div>
	<div id="tabsrdextension" class="tabcontent">
       {{page:SRD-Extension}}
    </div>
	<div id="tabsrdmsgdefinition" class="tabcontent">
       {{page:SRD-MessageDefinition}}
    </div>
	<div id="tabsrdcodesystem" class="tabcontent">
       {{page:SRD-CodeSystem}}
    </div>
	<div id="tabsrdvalueset" class="tabcontent">
       {{page:SRD-ValueSet}}
    </div>
  </div>
</div>
<br />
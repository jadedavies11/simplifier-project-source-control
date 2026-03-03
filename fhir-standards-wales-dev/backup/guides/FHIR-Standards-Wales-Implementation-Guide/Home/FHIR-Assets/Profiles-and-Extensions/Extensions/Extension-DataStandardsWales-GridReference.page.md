<div class="warning"><span class="ImplementWarn"></span></div>

## {{page-title}}
This extension captures a grid reference for the location as northings and eastings.

### Purpose
This extension extends the Location resource to support systems that use grid reference rather than longitude and latitude.

### Context of Use
This extension may be used on the following profile(s):
- Location

### Formal Views of Extension Content
<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openCity(this,'tabsnap')" data-target="tabsnap">
      Snapshot View
    </li>
    <li class="tablink" onclick="openCity(this,'tabeg')" data-target="tabeg">
      Example View
    </li>
  </ul>
  <div class="tab-main">
    <div id="tabsnap" class="tabcontent active">      
      {{tree:https://fhir.nhs.wales/StructureDefinition/Extension-DataStandardsWales-GridReference, snapshot}}
    </div>
    <div id="tabeg" class="tabcontent">
      <list>
         <li>Currently under development</li>
      </list>
    </div>
  </div>
</div>
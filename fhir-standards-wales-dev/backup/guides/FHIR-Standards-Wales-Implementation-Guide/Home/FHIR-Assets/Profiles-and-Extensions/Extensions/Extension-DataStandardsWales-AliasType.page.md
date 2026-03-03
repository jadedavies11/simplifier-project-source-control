<div class="warning"><span class="ImplementWarn"></span></div>

## {{page-title}}
This extension captures the nature of a recorded alias.

### Purpose
This extension extends the alias element of the Organization or Location resource to facilitate retrieval of specific types of alias that have a common use, for example short acronyms to be presented on charts.

### Context of Use
This extension may be used on the following elements:
- `Location.alias`
- `Organization.alias`

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/Extension-DataStandardsWales-AliasType, snapshot}}
    </div>
    <div id="tabeg" class="tabcontent">
      <list>
         <li>Currently under development</li>
      </list>
    </div>
  </div>
</div>
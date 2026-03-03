<div class="warning"><span class="ImplementWarn"></span></div>

## {{page-title}}
This extension captures the date range that this location should be considered available, irrespective of any availability exceptions within that period.

### Purpose
This extension extends the Location resource to indicate the date range for which the resource is valid as a health and/or cate location.

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/Extension-DataStandardsWales-LocationPeriod, snapshot}}
    </div>
    <div id="tabeg" class="tabcontent">
      <list>
         <li>Currently under development</li>
      </list>
    </div>
  </div>
</div>
## {{page-title}}
An extension to capture the national grid reference applicable to the location.

### Purpose
This extension shows tha national grid reference applicable to the location.  The grid reference resolves to a location on a map, which is found using the northing and easting numbered lines.

### Context of Use
This extension may be used on the following profile(s):
* Location

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
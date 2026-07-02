The following Terminologies have been defined for this Implementation Guide.

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openLocalTab(this,'bullet1')" data-target="bullet1">
    CodeSystems
    </li> 
    <li class="tablink" onclick="openLocalTab(this,'bullet2')" data-target="bullet2">
    ValueSets
    </li>
    <li class="tablink" onclick="openLocalTab(this,'narrative1')" data-target="narrative1">
    CodeSystems Narrative
    </li>
    <li class="tablink" onclick="openLocalTab(this,'narrative2')" data-target="narrative2">
    ValueSets Narrative
    </li>
    <li class="tablink" onclick="openLocalTab(this,'snomedct1')" data-target="snomedct1">
    ValueSets with SNOMED CT Codes
    </li>
    <li class="tablink" onclick="openLocalTab(this,'bullet3')" data-target="bullet3">
    CodeSystems in Profiles
    </li>
    <li class="tablink" onclick="openLocalTab(this,'bullet4')" data-target="bullet3">
    ValueSets in Profiles
    </li>
    <li class="tablink" onclick="openLocalTab(this,'exception1')" data-target="exception1">
    CodeSystem Exceptions
    </li>
    <li class="tablink" onclick="openLocalTab(this,'exception2')" data-target="exception1">
    ValueSet Exceptions
    </li>
     
  
  
  </ul>
  <div class="tab-main">
    <div id="bullet1" class="tabcontent active">
       {{page:BulletedList-CodeSystem}}
    </div>
    <div id="bullet2" class="tabcontent">
      {{page:BulletedList-ValueSet}} 
    </div>
    <div id="narrative1" class="tabcontent">
      {{page:Narrative-CodeSystem}} 
    </div>   
    <div id="narrative2" class="tabcontent">
      {{page:Narrative-ValueSet}} 
    </div>
    <div id="snomedct1" class="tabcontent">
       {{page:SCT-Codes-ValueSet}}
    </div>
    <div id="bullet3" class="tabcontent">
       {{page:BulletedList-CodeSystem-Profiles}}
    </div>
    <div id="bullet4" class="tabcontent">
       {{page:BulletedList-ValueSet-Profiles}}
    </div>
    <div id="exception1" class="tabcontent">
       {{page:Exception-CodeSystem}}
    </div>
    <div id="exception2" class="tabcontent">
       {{page:Exception-ValueSet}}
    </div>
 </div>
</div>

<script>
function openLocalTab(tabElement, tabId) {
  document.querySelectorAll('.tab-head .tablink').forEach(tab => {
    tab.classList.remove('tab-active');
  });

  document.querySelectorAll('.tab-main .tabcontent').forEach(content => {
    content.classList.remove('active');
  });

  tabElement.classList.add('tab-active');
  document.getElementById(tabId).classList.add('active');
}
</script>
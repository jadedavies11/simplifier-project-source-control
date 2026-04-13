The following Terminologies have been defined for this implementation guide.

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openLocalTab(this,'alphabetical')" data-target="alphabetical">
      Alphabetically listed ValueSets
    </li>
    <li class="tablink tab-active" onclick="openLocalTab(this,'bullet')" data-target="bullet">
      Simple ValueSet List
    </li>
    <li class="tablink" onclick="openLocalTab(this,'bullet2')" data-target="bullet2">
      ValueSets by Resource
    </li> 
    <li class="tablink" onclick="openLocalTab(this,'alphabetical2')" data-target="alphabetical2">
      Alphabetically listed CodeSystems
    </li>
    <li class="tablink" onclick="openLocalTab(this,'bullet3')" data-target="bullet3">
      Simple CodeSystem List
    </li>
    <li class="tablink" onclick="openLocalTab(this,'bullet4')" data-target="bullet4">
      CodeSystem by Resource
    </li>
    <li class="tablink" onclick="openLocalTab(this,'snomedct')" data-target="snomedct">
      Welsh ValueSets with SNOMED CT Codes
    </li>
    <li class="tablink" onclick="openLocalTab(this,'ukcore')" data-target="ukcore">
      UKCore ValueSets with Welsh Data
    </li>   
    <li class="tablink" onclick="openLocalTab(this,'pas')" data-target="pas">
      PAS ValueSets
    </li>
     
  
  
  </ul>
  <div class="tab-main">
    <div id="alphabetical" class="tabcontent active">
      {{page: New-ValueSet-List}} 
    </div>
    <div id="bullet" class="tabcontent active">
      {{page: Bulleted-VS-List}} 
    </div>
    <div id="bullet2" class="tabcontent active">
      {{page: Bulleted-VS-List-in-Profiles}} 
    </div>
    <div id="alphabetical2" class="tabcontent">
       {{page:New-CodeSystem-List}}
    </div>
    <div id="bullet3" class="tabcontent">
       {{page:Bulleted-CS-List}}
    </div>
    <div id="bullet4" class="tabcontent">
       {{page:Bulleted-CS-List-in-Profiles}}
    </div>
    <div id="snomedct" class="tabcontent">
       {{page:Welsh-VS-with-SCT-Codes}}
    </div>
    <div id="ukcore" class="tabcontent">
       {{page:UKCore-VS-with-Welsh-CS}}
    </div>
    <div id="pas" class="tabcontent">
       {{page:PAS-VS}}
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
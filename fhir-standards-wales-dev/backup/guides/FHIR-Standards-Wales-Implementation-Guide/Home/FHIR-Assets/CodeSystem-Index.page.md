<div class="warning"><span class="ImplementWarn"></span></div>

### {{page-title}}

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openLocalTab(this,'bullet1')" data-target="bullet1">
    CodeSystems
    </li> 
    <li class="tablink" onclick="openLocalTab(this,'narrative1')" data-target="narrative1">
    CodeSystems Narrative
    </li>
    <li class="tablink" onclick="openLocalTab(this,'bullet3')" data-target="bullet3">
    CodeSystems in Profiles
    </li>
    <li class="tablink" onclick="openLocalTab(this,'exception1')" data-target="exception1">
    CodeSystem Other Uses
    </li>
     
  
  
  </ul>
  <div class="tab-main">
    <div id="bullet1" class="tabcontent active">
       {{page:BulletedList-CodeSystem}}
    </div>
    <div id="narrative1" class="tabcontent">
      {{page:Narrative-CodeSystem}} 
    </div>   
    <div id="bullet3" class="tabcontent">
       {{page:BulletedList-CodeSystem-Profiles}}
    </div>
    <div id="exception1" class="tabcontent">
       {{page:Exception-CodeSystem}}
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
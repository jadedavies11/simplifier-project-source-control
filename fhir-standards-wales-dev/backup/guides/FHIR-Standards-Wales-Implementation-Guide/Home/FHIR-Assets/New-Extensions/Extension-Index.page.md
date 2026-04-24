### {{page-title}}

The following Extensions have been defined for this implementation guide.

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink" onclick="openLocalTab(this,'Extension-alphabetical')" data-target="Extension-alphabetical">
    Alphabetical
    </li> 
    <li class="tablink tab-active" onclick="openLocalTab(this,'Extension-narrative')" data-target="Extension-narrative">
    Narrative
    </li>
    <li class="tablink" onclick="openLocalTab(this,'Extension-resource')" data-target="Extension-resource">
    By Resource
    </li>
    <li class="tablink tab-active" onclick="openLocalTab(this,'UKCore-extension')" data-target="UKCore-extension">
    UK Core Extensions with Welsh Data
    </li>
    <li class="tablink" onclick="openLocalTab(this,'backport')" data-target="backport">
    R5 Backports
    </li>
     
  
  
  </ul>
  <div class="tab-main">
    <div id="Extension-alphabetical" class="tabcontent">
       {{page: Alphabetical-Extensions}}
    </div>
    <div id="Extension-narrative" class="tabcontent active">
      {{page: New-Extension}}
    </div>
    <div id="Extension-resource" class="tabcontent">
       {{page:Extensions-Modules}}
    </div>
    <div id="UKCore-extension" class="tabcontent active">
      {{page:Extensions-with-Welsh-Coded-Assets}} 
    </div>
    <div id="backport" class="tabcontent">
       {{page:R5-Backports}}
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




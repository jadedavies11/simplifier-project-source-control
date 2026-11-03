### {{page-title}}

This page describes the published versions of this implementation guide and differences between versions:

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openLocalTab(this,'list2')" data-target="list2">
    2.0.0 Release Notes
    </li>
    <li class="tablink" onclick="openLocalTab(this,'list1')" data-target="list1">
    1.0.0 Release Notes
    </li>
    <li class="tablink" onclick="openLocalTab(this,'discovery')" data-target="discovery">
    Discovery and Pre-ballot
    </li>
  </ul>

  
  <div class="tab-main">
    <div id="list2" class="tabcontent active">
      {{page:Release-List-2.0.0}} 
    </div>  
    <div id="list1" class="tabcontent">
      {{page:Release-List-1.0.0}} 
    </div>
    <div id="discovery" class="tabcontent">
       {{page:Discovery-Pre-ballot}}
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
</script
### {{page-title}}

The following Profiles have been defined for this implementation guide.

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openLocalTab(this,'alphabetical')" data-target="alphabetical">
      Alphabetical
    </li>
    <li class="tablink" onclick="openLocalTab(this,'resources')" data-target="resources">
      By Resources
    </li>
    <li class="tablink" onclick="openLocalTab(this,'active')" data-target="active">
      Active Profiles
    </li> 
    <li class="tablink" onclick="openLocalTab(this,'draft')" data-target="draft">
      Draft Profiles
    </li> 
  </ul>

  <div class="tab-main">
    <div id="alphabetical" class="tabcontent active">
       {{page: New-Profile}}
    </div>
    <div id="resources" class="tabcontent">
       {{page:Profiles-Modules}}
    </div>
  </div>
    <div id="active" class="tabcontent">
       {{page:Active-Profiles}}
    </div>
  </div>
      <div id="draft" class="tabcontent">
       {{page:Draft-Profiles}}
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

<style>
.tabcontent { display: none; }
.tabcontent.active { display: block; }
</style>
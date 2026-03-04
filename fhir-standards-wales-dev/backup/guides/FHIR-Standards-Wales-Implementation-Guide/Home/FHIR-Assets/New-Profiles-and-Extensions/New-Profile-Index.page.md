The following Profiles have been defined for this implementation guide.

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openLocalTab(this,'alphabetical')" data-target="alphabetical">
      Alphabetical
    </li>
    <li class="tablink" onclick="openLocalTab(this,'resources')" data-target="resources">
      By Resources
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
The following Extensions have been defined for this implementation guide.

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openLocalTab(this,'alphabetical')" data-target="alphabetical">
      Alphabetical
    </li>
    <li class="tablink" onclick="openLocalTab(this,'extension')" data-target="extension">
      Welsh Extensions in Profiles
    </li>
    <li class="tablink" onclick="openLocalTab(this,'extension2')" data-target="extension2">
      Extensions with Welsh Data
    </li>   
    <li class="tablink" onclick="openLocalTab(this,'backport')" data-target="backport">
      R5 Backports
    </li>  
  </ul>
  <div class="tab-main">
    <div id="alphabetical" class="tabcontent active">
      {{page: New-Extension}} 
    </div>
    <div id="extension" class="tabcontent">
       {{page:DSW-Profile-with-Welsh-Extensions}}
    </div>
    <div id="extension2" class="tabcontent">
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

<style>
.tabcontent { display: none; }
.tabcontent.active { display: block; }
</style>

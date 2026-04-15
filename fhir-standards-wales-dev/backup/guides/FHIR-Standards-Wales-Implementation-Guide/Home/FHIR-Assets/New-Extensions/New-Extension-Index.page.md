### {{page-title}}

The following Extensions have been defined for this implementation guide.

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openLocalTab(this,'narrative')" data-target="narrative">
      Narrative
    </li>
        <li class="tablink tab-active" onclick="openLocalTab(this,'alphabetical2')" data-target="alphabetical2">
      Alphabetical
    </li>
    <li class="tablink" onclick="openLocalTab(this,'extension')" data-target="extension">
      By Resource
    </li>
    <li class="tablink" onclick="openLocalTab(this,'extension2')" data-target="extension2">
      UK Core Extensions with Welsh Data
    </li>   
    <li class="tablink" onclick="openLocalTab(this,'backport')" data-target="backport">
      R5 Backports
    </li>  
  </ul>
  <div class="tab-main">
    <div id="narrative" class="tabcontent active">
      {{page: New-Extension}} 
    </div>
        <div id="alphabetical2" class="tabcontent active">
      {{page: Alphabetical-Extensions}} 
    </div>
    <div id="extension" class="tabcontent">
       {{page:Extensions-Modules}}
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


### {{page-title}}

This page presents a tabulated view of release notes. The release notes provide detailed information on the changes introduced in a specific release. For additional context, including links to the published Implementation Guides, FHIR packages, and a complete history of all releases, please refer to the Version History section of [Wales FHIR Implementation Guide Version History](https://simplifier.net/guide/wales-fhir-implementation-guide-version-history)<br>
<br>For a consolidated view of Release Notes, please refer to {{pagelink:Complete-ReleaseNotes, text:Complete Release Notes}}<br>


<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" data-tab="list2">Versions 2.n.n</li>
    <li class="tablink" data-tab="list1">Versions 1.n.n</li>
    <li class="tablink" data-tab="discovery">Discovery and Pre-ballot</li>
    <li class="tablink" data-tab="full">List of Release Notes</li>
  </ul>
  <div class="tab-main">
    <div id="list2" class="tabcontent active">{{page:ReleaseList-releaseTwo}}</div>
    <div id="list1" class="tabcontent">{{page:ReleaseList-releaseOne}}</div>
    <div id="discovery" class="tabcontent">{{page:Discovery-List}}</div>
    <div id="full" class="tabcontent">{{page:List-of-all-Release-Notes}}</div>
  </div>
</div>
<br><br><br>
<script>
document.addEventListener("DOMContentLoaded", function () {
  const tabs = document.querySelectorAll('.tablink');
  tabs.forEach(tab => {
    tab.addEventListener("click", function () {
      document.querySelectorAll('.tablink').forEach(t => t.classList.remove('tab-active'));
      document.querySelectorAll('.tabcontent').forEach(c => c.classList.remove('active'));
      this.classList.add('tab-active');
      document.getElementById(this.dataset.tab).classList.add('active');
    });
  });
  document.querySelector('.tablink.tab-active')?.click();
});
</script>
<br><br>
<style>
.tabcontent { display: none; }
.tabcontent.active { display: block; }
.tablink { cursor: pointer; }
.tab-active { font-weight: bold; }
</style>
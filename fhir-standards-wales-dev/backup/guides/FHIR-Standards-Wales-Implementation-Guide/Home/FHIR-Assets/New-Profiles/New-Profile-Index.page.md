### {{page-title}}

The following Profiles have been defined for this implementation guide.

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink" data-tab="alphabetical">Alphabetical</li>
    <li class="tablink tab-active" data-tab="resources">By Resources</li>
    <li class="tablink" data-tab="status1">Profiles (Active)</li>
    <li class="tablink" data-tab="status2">Profiles (Draft)</li>
  </ul>

  <div class="tab-main">
    <div id="alphabetical" class="tabcontent">{{page:New-Profile}}</div>
    <div id="resources" class="tabcontent active">{{page:Profiles-Category}}</div>
    <div id="status1" class="tabcontent">{{page:Live-Profiles}}</div>
    <div id="status2" class="tabcontent">{{page:Draft-Profiles}}</div>
  </div>
</div>

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

<style>
.tabcontent { display: none; }
.tabcontent.active { display: block; }
.tablink { cursor: pointer; }
.tab-active { font-weight: bold; }
</style>
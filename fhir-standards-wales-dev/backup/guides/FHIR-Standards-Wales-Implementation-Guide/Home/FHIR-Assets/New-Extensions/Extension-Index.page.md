### {{page-title}}


<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" data-tab="Extension-alphabetical">Alphabetical</li> 
    <li class="tablink" data-tab="Extension-narrative">Narrative</li>
    <li class="tablink" data-tab="Extension-resource">By Resource</li>
    <li class="tablink" data-tab="DSW-extension">Profiles with Welsh Extensions</li>
    <li class="tablink" data-tab="UKCore-extension">UK Core Extensions with Welsh Data</li>
     
  
  
  </ul>
  <div class="tab-main">
    <div id="Extension-alphabetical" class="tabcontent">
       {{page:Alphabetical-Extensions}}
    </div>
    <div id="Extension-narrative" class="tabcontent active">
      {{page:Extension-Narrative}}
    </div>
    <div id="Extension-resource" class="tabcontent">
       {{page:Extensions-Resource}}
    </div>
        <div id="DSW-extension" class="tabcontent">
       {{page:DSW-Profile-with-Welsh-Extensions}}
    </div>
    <div id="UKCore-extension" class="tabcontent active">
      {{page:Extensions-WelshData}} 
    </div>
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
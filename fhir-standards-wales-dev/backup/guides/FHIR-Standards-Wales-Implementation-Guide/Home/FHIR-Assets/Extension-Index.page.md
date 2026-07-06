<div class="warning"><span class="ImplementWarn"></span></div>

### {{page-title}}


<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" data-tab="Extension-alphabetical">Alphabetical</li> 
    <li class="tablink" data-tab="Extension-profile">By Profile</li>
    <li class="tablink" data-tab="Extension-terminologies">With Terminologies</li>
    <li class="tablink" data-tab="UKCore-extension">UK Core Extensions with Welsh Terminologies</li>
  
  
  
  </ul>
  <div class="tab-main">
    <div id="Extension-alphabetical" class="tabcontent active">{{page:Alphabetical-Extensions}}</div>
    <div id="Extension-profile" class="tabcontent">{{page:Profile-Extensions}}</div>
    <div id="Extension-terminologies" class="tabcontent">{{page:Terminology-Extensions}}</div>
    <div id="UKCore-extension" class="tabcontent">{{page:UKCore-Extensions-WelshTerminologies}}</div>
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
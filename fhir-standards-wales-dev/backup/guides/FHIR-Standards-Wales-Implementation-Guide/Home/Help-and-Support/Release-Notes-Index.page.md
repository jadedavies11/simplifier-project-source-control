
### {{page-title}}

This page describes the published versions of this implementation guide and differences between versions:

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" data-tab="list2">2.0.0 Release Notes</li> 
    <li class="tablink" data-tab="list1">1.0.0 Release Notes</li>
    <li class="tablink" data-tab="discovery">Discovery and Pre-ballot</li>
  
  
  
  </ul>
  <div class="tab-main">
    <div id="list2" class="tabcontent active">{{page:Release-List-2.0.0}}</div>
    <div id="list1" class="tabcontent">{{page:Release-List-1.0.0}}</div>
    <div id="discovery" class="tabcontent">{{page:Release-List-0.0.1}}</div>
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
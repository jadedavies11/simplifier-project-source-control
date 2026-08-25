## Example DocumentReference - Potentially Misfiled
This DocumentReference example illustrates the first step of the {{pagelink:Document-Error-Workflow, text:document misfile workflow}}. It shows the effect on the DocumentReference resource of a user proposing that the document represented by {{pagelink:Example-DataStandardsWales-DocumentReference-EventBased, text:Example DocumentReference - Event-based}} has been misfiled i.e. added to the wrong patient. The details of the proposal can be found in the corresponding Task resource{{pagelink:Example-DataStandardsWales-Task-MisfileRequested, text:Example Task - Misfile Rejected}}.

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink" onclick="openCity(this,'tabtree')" data-target="tabtree">
      Overview
    </li>
    <li class="tablink" onclick="openCity(this,'tabtable')" data-target="tabtable">
      Table
    </li>
    <li class="tablink tab-active" onclick="openCity(this,'tabxml')" data-target="tabxml">
      XML
    </li>    
    <li class="tablink" onclick="openCity(this,'tabjson')" data-target="tabjson">
      JSON
    </li>    
  </ul>
  <div class="tab-main">
    <div id="tabtree" class="tabcontent">
      {{tree:DocumentReference/Example-DataStandardsWales-DocumentReference-PotentiallyMisfiled}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:DocumentReference/Example-DataStandardsWales-DocumentReference-PotentiallyMisfiled}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:DocumentReference/Example-DataStandardsWales-DocumentReference-PotentiallyMisfiled}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:DocumentReference/Example-DataStandardsWales-DocumentReference-PotentiallyMisfiled}}
    </div>        
  </div>
</div>
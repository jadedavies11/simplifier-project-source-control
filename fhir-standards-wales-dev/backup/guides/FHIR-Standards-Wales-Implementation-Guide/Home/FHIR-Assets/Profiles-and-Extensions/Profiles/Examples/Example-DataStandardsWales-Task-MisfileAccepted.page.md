## Example Task - Misfile Accepted
This Task example illustrates the second step of the {{pagelink:Document-Error-Workflow, text:document misfile workflow}} in the case that the misfile review outcome was "accepted". It builds on the misfile requested example {{pagelink:Example-DataStandardsWales-Task-MisfileRequested, text:Example Task - Misfile Requested}} to add details of when (`lastModified`), why (`note.text`) and by whom (`owner`) the proposed document misfile was accepted.

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
      {{tree:Example-DataStandardsWales-Task-MisfileAccepted}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:Example-DataStandardsWales-Task-MisfileAccepted}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:Example-DataStandardsWales-Task-MisfileAccepted}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:Example-DataStandardsWales-Task-MisfileAccepted}}
    </div>        
  </div>
</div>
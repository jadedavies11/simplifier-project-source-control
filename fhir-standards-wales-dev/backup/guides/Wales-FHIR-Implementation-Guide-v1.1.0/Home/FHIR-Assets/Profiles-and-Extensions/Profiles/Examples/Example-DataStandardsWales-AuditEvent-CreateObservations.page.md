## {{page-title}}

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
    <li class="tablink" onclick="openCity(this,'tabnarrative')" data-target="tabnarrative">
      Narrative
    </li>
  </ul>
  <div class="tab-main">
    <div id="tabtree" class="tabcontent">
      {{tree:AuditEvent/Example-AuditEvent-CreateObservations}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:AuditEvent/Example-AuditEvent-CreateObservations}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:AuditEvent/Example-AuditEvent-CreateObservations}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:AuditEvent/Example-AuditEvent-CreateObservations}}
    </div>       
    <div id="tabnarrative" class="tabcontent">
      {{narrative:AuditEvent/Example-AuditEvent-CreateObservations}}
    </div>  
  </div>
</div>
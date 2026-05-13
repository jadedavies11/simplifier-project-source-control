## Example Document Reference - Misfiled (document not event-based)
This example represents a document which has been misfiled via a two-step workflow: misfile proposed and then accepted.  The document in this example is not based on a patient healthcare event.

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
      {{tree:Example-DSW-DocumentReference-MisfiledNotEventBased}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:Example-DSW-DocumentReference-MisfiledNotEventBased}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:Example-DSW-DocumentReference-MisfiledNotEventBased}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:Example-DSW-DocumentReference-MisfiledNotEventBased}}
    </div>       
    <div id="tabnarrative" class="tabcontent">
      {{narrative:Example-DSW-DocumentReference-MisfiledNotEventBased}}
    </div>  
  </div>
</div>
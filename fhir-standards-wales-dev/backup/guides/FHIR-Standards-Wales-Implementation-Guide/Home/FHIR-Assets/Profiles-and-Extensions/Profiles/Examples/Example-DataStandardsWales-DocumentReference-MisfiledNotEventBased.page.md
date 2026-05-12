## Example Document Reference - Misfiled (document not event-based)
This example illustrates a document reference that represents the misfiling of the example document in {{pagelink:Example-DataStandardsWales-DocumentReference-NotEventBased, text: Example Document Reference - Not event-based}}.  In this scenario the original document was erroneously recorded against the prior patient seen.  The `errorAction` extension has been used to record the steps in the misfiling workflow: in which a nurse noticed the error and proposed the misfile, then subsequently the misfile was reviewed and accepted by a consultant.  The `status` and `errorStatus` have been updated accordingly.

NOTE that the example is illustrative of DocumentReference content in a misfile scenario.  Not all of the referenced resources currently exist as examples within this implementation guide.

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
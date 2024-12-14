## {{page-title}}
This Provenance example demonstrates how logical references can be used where Device resources are not available in within the data store.

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
      {{tree:Provenance/Example-DataStandardsWales-Provenance-Amend-Alt}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:Provenance/Example-DataStandardsWales-Provenance-Amend-Alt}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:Provenance/Example-DataStandardsWales-Provenance-Amend-Alt}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:Provenance/Example-DataStandardsWales-Provenance-Amend-Alt}}
    </div>       
    <div id="tabnarrative" class="tabcontent">
      {{narrative:Provenance/Example-DataStandardsWales-Provenance-Amend-Alt}}
    </div>  
  </div>
</div>
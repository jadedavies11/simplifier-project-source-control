## Example Endpoint - Radiology DICOM Endpoint

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
      {{tree:Endpoint/Example-Endpoint-Dicom}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:Endpoint/Example-Endpoint-Dicom}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:Endpoint/Example-Endpoint-Dicom}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:Endpoint/Example-Endpoint-Dicom}}
    </div>       
    <div id="tabnarrative" class="tabcontent">
      {{narrative:Endpoint/Example-Endpoint-Dicom}}
    </div>  
  </div>
</div>
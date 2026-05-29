## Example Practitioner - Joe Bloggs (Consultant)

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
      {{tree:Practitioner/Example-DSW-Practitioner-Consultant-JoeBloggs}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:Practitioner/Example-DSW-Practitioner-Consultant-JoeBloggs}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:Practitioner/Example-DSW-Practitioner-Consultant-JoeBloggs}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:Practitioner/Example-DSW-Practitioner-Consultant-JoeBloggs}}
    </div>       
    <div id="tabnarrative" class="tabcontent">
      {{narrative:Practitioner/Example-DSW-Practitioner-Consultant-JoeBloggs}}
    </div>  
  </div>
</div>
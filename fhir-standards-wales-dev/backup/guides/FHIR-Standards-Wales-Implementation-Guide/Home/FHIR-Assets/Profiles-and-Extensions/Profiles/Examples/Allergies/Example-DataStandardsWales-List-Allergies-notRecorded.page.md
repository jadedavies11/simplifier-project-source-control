<div class="warning"><span class="ClinicalWarn"></span></div>

## Example List - Empty Allergies List

This example references the following example resources:

* Subject, source and context:
  * {{pagelink:Example-DataStandardsWales-Patient-AliceJones, text:Patient - Alice Jones}}
  * {{pagelink:Example-DataStandardsWales-Practitioner-Consultant, text:Practitioner - Dr Dhiren Patel }}


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
      {{tree:Example-DataStandardsWales-List-Allergies-notRecorded}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:Example-DataStandardsWales-List-Allergies-notRecorded}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:Example-DataStandardsWales-List-Allergies-notRecorded}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:Example-DataStandardsWales-List-Allergies-notRecorded}}
    </div>       
    <div id="tabnarrative" class="tabcontent">
      {{narrative:Example-DataStandardsWales-List-Allergies-notRecorded}}
    </div>  
  </div>
</div>
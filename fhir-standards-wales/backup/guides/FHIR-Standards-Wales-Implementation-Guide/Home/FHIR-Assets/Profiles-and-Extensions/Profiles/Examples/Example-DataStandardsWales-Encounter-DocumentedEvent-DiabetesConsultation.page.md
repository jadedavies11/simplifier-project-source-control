## Example Encounter - Documented Event (Diabetes Consultation)
This example supports the illustration of an encounter-based DocumentReference.  It is referenced within {{pagelink:Example-DataStandardsWales-DocumentReference-EncounterBased, text:Example DocumentReference - Encounter-based}} as the Encounter context for the document. This Encounter carries the minimal dataset for document event data that would be expected if there was no dedicated application functionality to provide a fuller Encounter dataset.  

The Encounter specifically supports a document reference representing a diabetes consultation:
- The consultation occurred in the Outpatients Department of Glangwili General Hospital at 09:37 on 22nd July
- the senior responsible clinician was Dr Joe Bloggs 
- The service was provided by Hywel Dda University Local Health Board

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
      {{tree:Encounter/Example-DSW-Encounter-DocumentedEvent-DiabetesConsultation}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:Encounter/Example-DSW-Encounter-DocumentedEvent-DiabetesConsultation}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:Encounter/Example-DSW-Encounter-DocumentedEvent-DiabetesConsultation}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:Encounter/Example-DSW-Encounter-DocumentedEvent-DiabetesConsultation}}
    </div>       
    <div id="tabnarrative" class="tabcontent">
      {{narrative:Encounter/Example-DSW-Encounter-DocumentedEvent-DiabetesConsultation}}
    </div>  
  </div>
</div>
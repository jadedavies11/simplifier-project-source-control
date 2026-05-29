## Example Document Reference - Encounter-based
This document reference example represents a document from a patient consultation with the adult diabetes service that has been captured as an Encounter in the patient record.  The patient was seen by a nurse and a dietitian, who both authored content within the document.  The document was finalised and approved by the consultant with overall responsibility for the patient's care.  The document content is signposted by a url to the location from which the document PDF can be retrieved for display.

NOTE that the example is illustrative of DocumentReference content in the case that an Encounter exists.  That Encounter holds the document metadata items that relate to the event such as event location and senior responsible clinician.  Not all of the referenced resources currently exist as examples within this implementation guide.

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
      {{tree:DocumentReference/Example-DataStandardsWales-DocumentReference-EncounterBased}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:DocumentReference/Example-DataStandardsWales-DocumentReference-EncounterBased}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:DocumentReference/Example-DataStandardsWales-DocumentReference-EncounterBased}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:DocumentReference/Example-DataStandardsWales-DocumentReference-EncounterBased}}
    </div>       
    <div id="tabnarrative" class="tabcontent">
      {{narrative:DocumentReference/Example-DataStandardsWales-DocumentReference-EncounterBased}}
    </div>  
  </div>
</div>
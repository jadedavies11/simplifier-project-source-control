## Example Medications List - Discharge medication

This example medication list is provided as part of a patient journey scenario, which is described {{pagelink:Home/Guidance/Medications/Index.page.md, text:here}}. The list references the following example resources:
* Subject, source and context:
  * {{pagelink:Example-DataStandardsWales-Patient-PeterPiper, text:Example Patient - Peter Piper}}
* Medication statements:
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Atorva.-Discharge, text:Example MedicationStatement - Discharge - Atorvastatin}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Bendro.-Discharge, text:Example MedicationStatement - Discharge - Bendroflumethiazide}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Bisop.-Discharge, text:Example MedicationStatement - Discharge - Bisoprolol}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Duroge.-Discharge, text:Example MedicationStatement - Discharge - Durogesic DTrans}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Enbrel-Discharge, text:Example MedicationStatement - Discharge - Enbrel}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Hydroc.-Discharge, text:Example MedicationStatement - Discharge - Hydrocortisone}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Latano.-Discharge, text:Example MedicationStatement - Discharge - Latanoprost}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Nifedi.-Discharge, text:Example MedicationStatement - Discharge - Nifedipress}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Parace.-Discharge, text:Example MedicationStatement - Discharge - Paracetamol}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Ramipri.-Discharge, text:Example MedicationStatement - Discharge - Ramipril}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Ibupro.-Discharge, text:Example MedicationStatement - Discharge - Ibuprofen (stopped)}}

Below is an example of the above medication statements combined into a medication list:
  
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
      {{tree:example-datastandardswales-medicationlist-discharge}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:example-datastandardswales-medicationlist-discharge}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:example-datastandardswales-medicationlist-discharge}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:example-datastandardswales-medicationlist-discharge}}
    </div>       
    <div id="tabnarrative" class="tabcontent">
      {{narrative:example-datastandardswales-medicationlist-discharge}}
    </div>  
  </div>
</div>
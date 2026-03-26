## Example Medications List - Inpatient medication

This example medication list is provided as part of a patient journey scenario, which is described {{pagelink:Home/Guidance/Medications/Index.page.md, text:here}}. The list references the following example resources:
* Subject, source and context:
  * {{pagelink:Example-DataStandardsWales-Patient-PeterPiper, text:Example Patient - Peter Piper}}
* Medication statements:
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Atorva.-Inpatient, text:Example MedicationStatement - Inpatient - Atorvastatin}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Bendro.-Inpatient, text:Example MedicationStatement - Inpatient - Bendroflumethiazide}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Bisop.-Inpatient, text:Example MedicationStatement - Inpatient - Bisoprolol}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Duroge.-Inpatient, text:Example MedicationStatement - Inpatient - Durogesic DTrans}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Enbrel-Inpatient, text:Example MedicationStatement - Inpatient - Enbrel}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Hydroc.-Inpatient, text:Example MedicationStatement - Inpatient - Hydrocortisone}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Latano.-Inpatient, text:Example MedicationStatement - Inpatient - Latanoprost}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Nifedi.-Inpatient, text:Example MedicationStatement - Inpatient - Nifedipress}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Parace.-Inpatient, text:Example MedicationStatement - Inpatient - Paracetamol}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Ramipr.-Inpatient, text:Example MedicationStatement - Inpatient - Ramipril}}
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Ibupro.-Inpatient, text:Example MedicationStatement - Inpatient - Ibuprofen (stopped)}}
  
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
      {{tree:example-datastandardswales-list-medications-inpatient}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:example-datastandardswales-list-medications-inpatient}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:example-datastandardswales-list-medications-inpatient}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:example-datastandardswales-list-medications-inpatient}}
    </div>       
    <div id="tabnarrative" class="tabcontent">
      {{narrative:example-datastandardswales-list-medications-inpatient}}
    </div>  
  </div>
</div>
## Example Medications List - Medicines on admission

This example medication list is provided as part of a patient journey scenario, which is described {{pagelink:Home/Guidance/Medications/Index.page.md, text:here}}. The list references the following example resources:
* Subject, source and context:
  * {{pagelink:Example-Patient-PeterPiper, text:Example Patient - Peter Piper}}
* Medication statements:
  * {{pagelink:Example-MedicationStatement-Amoxicillin-GP, text:Example MedicationStatement - GP - Amoxicillin}}
  * {{pagelink:Example-MedicationStatement-Atorvastatin-GP, text:Example MedicationStatement - GP - Atorvastatin}}
  * {{pagelink:Example-MedicationStatement-Bendro.-GP, text:Example MedicationStatement - GP - Bendroflumethiazide}}
  * {{pagelink:Example-MedicationStatement-Bisoprolol-GP, text:Example MedicationStatement - GP - Bisoprolol}}
  * {{pagelink:Example-MedicationStatement-DurogesicDTrans-GP, text:Example MedicationStatement - GP - Durogesic DTrans}}
  * {{pagelink:Example-MedicationStatement-Hydrocortisone-GP, text:Example MedicationStatement - GP - Hydrocortisone}}
  * {{pagelink:Example-MedicationStatement-Latanoprost-GP, text:Example MedicationStatement - GP - Latanoprost}}
  * {{pagelink:Example-MedicationStatement-Nifedipress-GP, text:Example MedicationStatement - GP - Nifedipress}}
  * {{pagelink:Example-MedicationStatement-Ramipril-GP, text:Example MedicationStatement - GP - Ramipril}}
  * {{pagelink:Example-MedicationStatement-Enbrel-Outpatient, text:Example MedicationStatement - Outpatient - Enbrel}}
  * {{pagelink:Example-MedicationStatement-Ibupro.-Admission, text:Example MedicationStatement - Patient reported - Ibuprofen}}
  * {{pagelink:Example-MedicationStatement-Parace.-Admission, text:Example MedicationStatement - Patient reported - Paracetamol}}

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
      {{tree:List/Example-MedicationList-Admission}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:List/Example-MedicationList-Admission}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:List/Example-MedicationList-Admission}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:List/Example-MedicationList-Admission}}
    </div>       
    <div id="tabnarrative" class="tabcontent">
      {{narrative:List/Example-MedicationList-Admission}}
    </div>  
  </div>
</div>
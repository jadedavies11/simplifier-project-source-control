## Example Medications List - Rheumatology Clinic

This example medication list is provided as part of a patient journey scenario, which is described {{pagelink:Home/Guidance/Medications/Index.page.md, text:here}}. The list references the following example resources:
* Subject, source and context:
  * {{pagelink:Example-DataStandardsWales-Patient-PeterPiper, text:Example Patient - Peter Piper}}
* Medication statements:
  * {{pagelink:Example-DataStandardsWales-MedicationStatement-Enbrel-Outpatient, text:Example MedicationStatement - Outpatient - Enbrel}}

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
      {{tree:Example-DataStandardsWales-MedicationList-Outpatient}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:Example-DataStandardsWales-MedicationList-Outpatient}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:Example-DataStandardsWales-MedicationList-Outpatient}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:Example-DataStandardsWales-MedicationList-Outpatient}}
    </div>       
    <div id="tabnarrative" class="tabcontent">
      {{narrative:Example-DataStandardsWales-MedicationList-Outpatient}}
    </div>  
  </div>
</div>
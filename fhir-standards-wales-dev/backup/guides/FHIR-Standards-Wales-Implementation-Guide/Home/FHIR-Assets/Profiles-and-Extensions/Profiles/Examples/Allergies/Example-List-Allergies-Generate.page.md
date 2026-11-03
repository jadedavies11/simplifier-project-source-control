## Example Allergy List - Generate

This example references the following example resources:
* Allergies:
  * {{pagelink:Example-AllergyIntolerance-Aspirin, text:Example AllergyIntolerance - Medication (aspirin)}}
  * {{pagelink:Example-AllergyIntolerance-Morphine, text:Example AllergyIntolerance - Medication (morphine)}} - following modification from degraded to be coded correctly
  * {{pagelink:Example-AllergyIntolerance-Potato, text:Example AllergyIntolerance - Food (potato)}}
  * {{pagelink:Example-AllergyIntolerance-Ibuprofen, text:Example AllergyIntolerance - Medication (ibuprofen)}} - following modification from degraded to be coded correctly
  * {{pagelink:Example-AllergyIntolerance-Wasps, text:Example AllergyIntolerance - Wasps}} - following modification from degraded to be coded correctly
  
* Subject, source and context:
  * {{pagelink:Example-Patient-AliceJones, text:Example Patient - Alice Jones}}
  * {{pagelink:Example-Practitioner-Consultant, text:Example Practitioner - Dhiren Patel (Consultant)}}


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

  </ul>
  <div class="tab-main">
    <div id="tabtree" class="tabcontent">
      {{tree:List/Example-List-Allergies-Generate}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:List/Example-List-Allergies-Generate}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:List/Example-List-Allergies-Generate}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:List/Example-List-Allergies-Generate}}
    </div>       
  </div>
</div>
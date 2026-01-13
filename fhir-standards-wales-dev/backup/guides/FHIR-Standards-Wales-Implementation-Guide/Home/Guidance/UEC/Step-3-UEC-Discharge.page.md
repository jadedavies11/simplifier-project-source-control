The final data submission occurs after the patient has been discharged at the UEC facility.

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openLocalTab(this,'tabnarrative3')" data-target="tabnarrative3">
      Step Narrative
    </li>
    <li class="tablink" onclick="openLocalTab(this,'tabstepdata3')" data-target="tabstepdata3">
      Step Data
    </li>
    <li class="tablink" onclick="openLocalTab(this,'tabdatamodel3')" data-target="tabdatamodel3">
      Messaging Data Model
    </li>   
    <li class="tablink" onclick="openLocalTab(this,'tabmsgdefinition3')" data-target="tabmsgdefinition3">
      Message Definition
    </li>  
    <li class="tablink" onclick="openLocalTab(this,'tabbundle3')" data-target="tabbundle3">
      Example Bundle
    </li>  
  </ul>
  <div class="tab-main">
    <div id="tabnarrative3" class="tabcontent active">
       Marjorie was seen by a health care assistant and a consultant during the visit, the first at 12:30. The consultations resulted in a diagnosis of a sprained ankle and appropriate management, before Marjorie was discharged to home at 14:35, with advice for follow-up via her general practitioner. A copy of the discharge letter was provided to her at the point of discharge.
    </div>
    <div id="tabstepdata3" class="tabcontent">
       {{page:Step-3-UEC-Discharge-Data}}
    </div>
    <div id="tabdatamodel3" class="tabcontent">
       {{render:Diagrams-UEC-discharge-messaging-model}}
    </div>
    <div id="tabmsgdefinition3" class="tabcontent">
       An XML rendering of the message definition is shown below.  See the dedicated message definition page for JSON and other representations: {{pagelink:MessageDefinition-DataStandardsWales-UEC-Discharge}}<br /><br />
       {{xml:MessageDefinition/MessageDefinition-DataStandardsWales-UEC-Discharge}}
    </div>
    <div id="tabbundle3" class="tabcontent">
       An XML rendering of the example message bundle is shown below.  See the dedicated example page for JSON and other representations: {{pagelink:Example-DataStandardsWales-Bundle-UEC-Discharge-UHWEUMI, text: Example Message Bundle - UEC Discharge UHWEUMI (UHW Emergency Unit Minor Injuries)}}<br /><br />
       {{xml:Example-DataStandardsWales-Bundle-UEC-Discharge-UHWEUMI}}
    </div>
  </div>
</div>
<br />
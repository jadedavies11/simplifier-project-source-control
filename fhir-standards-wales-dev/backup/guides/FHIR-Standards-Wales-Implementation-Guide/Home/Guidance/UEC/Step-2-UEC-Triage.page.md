The second data submission occurs after the patient has been triaged at the UEC facility and the acuity of the attendance determined.

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openCity(this,'tabnarrative2')" data-target="tabnarrative2">
      Step Narrative
    </li>
    <li class="tablink" onclick="openCity(this,'tabstepdata2')" data-target="tabstepdata2">
      Step Data
    </li>
    <li class="tablink" onclick="openCity(this,'tabdatamodel2')" data-target="tabdatamodel2">
      Messaging Data Model
    </li>   
    <li class="tablink" onclick="openCity(this,'tabmsgdefinition2')" data-target="tabmsgdefinition2">
      Message Definition
    </li>  
    <li class="tablink" onclick="openCity(this,'tabbundle2')" data-target="tabbundle2">
      Example Bundle
    </li>  
  </ul>
  <div class="tab-main">
    <div id="tabnarrative2" class="tabcontent active">
       At 12:12 Marjorie was assessed by triage nurse Mrs Lisa Potts as requiring standard level emergency care acuity and the swollen ankle was recorded together with the comorbidities of asthma and hypertension. 
    </div>
    <div id="tabstepdata2" class="tabcontent">
       {{page:Step-2-UEC-Triage-Data}}
    </div>
    <div id="tabdatamodel2" class="tabcontent">
       {{render:Diagrams-UEC-triage-messaging-model}}
    </div>
    <div id="tabmsgdefinition2" class="tabcontent">
       An XML rendering of the message definition is shown below.  See the dedicated message definition page for JSON and other representations: {{pagelink:MessageDefinition-DataStandardsWales-UEC-Triage}}<br /><br />
       {{xml:MessageDefinition/MessageDefinition-DataStandardsWales-UEC-Triage}}
    </div>
    <div id="tabbundle2" class="tabcontent">
       An XML rendering of the example message bundle is shown below.  See the dedicated example page for JSON and other representations: {{pagelink:Example-DataStandardsWales-Bundle-UEC-Triage-UHWEUMI, text: Example Message Bundle - UEC Triage UHWEUMI (UHW Emergency Unit Minor Injuries)}}<br /><br />
       {{xml:Example-DataStandardsWales-Bundle-UEC-Triage-UHWEUMI}}
    </div>
  </div>
</div>
<br />
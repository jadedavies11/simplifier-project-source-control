The first data submission occurs after the patient arrival at the UEC facility has been registered.  

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openCity(this,'tabnarrative1')" data-target="tabnarrative1">
      Step Narrative
    </li>
    <li class="tablink" onclick="openCity(this,'tabstepdata1')" data-target="tabstepdata1">
      Step Data
    </li>
    <li class="tablink" onclick="openCity(this,'tabdatamodel1')" data-target="tabdatamodel1">
      Messaging Data Model
    </li>   
    <li class="tablink" onclick="openCity(this,'tabmsgdefinition1')" data-target="tabmsgdefinition1">
      Message Definition
    </li>  
    <li class="tablink" onclick="openCity(this,'tabbundle1')" data-target="tabbundle1">
      Example Bundle
    </li>  
  </ul>
  <div class="tab-main">
    <div id="tabnarrative1" class="tabcontent active">
       Ms Marjorie Pryor attends the Emergency Unit Minor Injuries facility of University Hospital of Wales at 12:00 on 02/12/2025 with a painful swollen ankle. She has been advised to attend by her GP at North Cardiff Medical Centre and an appointment was booked for 12:15. She travelled to the appointment by bus. This was her first UEC attendance for the condition.
    </div>
    <div id="tabstepdata1" class="tabcontent">
       {{page:Step-1-UEC-Arrival-Data}}
    </div>
    <div id="tabdatamodel1" class="tabcontent">
       {{render:Diagrams-UEC-arrival-messaging-model}}
    </div>
    <div id="tabmsgdefinition1" class="tabcontent">
       An XML rendering of the message definition is shown below.  See the dedicated message definition page for JSON and other representations: {{pagelink:MessageDefinition-DataStandardsWales-UEC-Arrival}}<br /><br />
       {{xml:MessageDefinition/MessageDefinition-DataStandardsWales-UEC-Arrival}}
    </div>
    <div id="tabbundle1" class="tabcontent">
       An XML rendering of the example message bundle is shown below.  See the dedicated example page for JSON and other representations: {{pagelink:Example-DataStandardsWales-Bundle-UEC-Arrival-UHWEUMI, text: Example Message Bundle - UEC Arrival UHWEUMI (UHW Emergency Unit Minor Injuries)}}<br /><br />
       {{xml:Example-DataStandardsWales-Bundle-UEC-Arrival-UHWEUMI}}
    </div>
  </div>
</div>
<br />
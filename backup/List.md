## List

The Child Protection Information Sharing implementation uses the StructureDefinition List profiled as UKCore-List:

## UKCore-List ##

<div class="tab">
  <button class="tablinks" onclick="openTab(event, 'Differential View')">Differential View</button>
  <button class="tablinks active" onclick="openTab(event, 'Hybrid View')">Hybrid View</button>
  <button class="tablinks" onclick="openTab(event, 'Snapshot View')">Snapshot View</button>
  <button class="tablinks" onclick="openTab(event, 'Examples')">Examples</button>
</div>

<div id="Differential View" class="tabcontent">
  <h3>Differential View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-List, diff}}
</div>

<div id="Hybrid View" class="tabcontent" style="display:block">
  <h3>Hybrid View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-List, hybrid}}
</div>

<div id="Snapshot View" class="tabcontent">
  <h3>Snapshot View</h3>
 {{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-List, snapshot}}
</div>

<div id="Examples" class="tabcontent">
  <h3>Examples</h3>
There are currently no specific CP-IS examples for List. 

</div>


 ## Conformance Rules

 ### CarePlan List   

| Source data item       | Cardinality | Target FHIR element                          | Conformance rules                                                                                                                                                                             |
|------------------------|-------------|----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Total returned plans | 1..1        | Extension-CPIS-TotalCarePlans.valuePositiveInt | This count will be carried in {{pagelink:ExtensionCPIS-TotalCarePlans}}.                                                                                                                        |
|                        | 1..1        | status                                       | Fixed value = <code>current</code>.                                                                                                                                                           |
|                        | 1..1        | mode                                         | Fixed value = <code>snapshot</code>.                                                                                                                                                          |
|                        | 1..1        | code                                         | Code.coding.system will be fixed to <code>http://snomed.info/sct</code>.<br>Code.coding.code will be fixed to <code>734163000</code>.<br>Code.coding.display will be fixed to <code>Care Plan</code>. |
|                        | 1..1        | subject                                      | This element will reference {{pagelink:Patient}}.                                                                                                                                              |
|                        | 1..*        | entry.item                                   | This element will reference {{pagelink:CarePlan}}.                                                                                                                                           |


 ### AuditEvent List   

| Source data item       | Cardinality | Target FHIR element                          | Conformance rules                                                                                                                                                                             |
|------------------------|-------------|----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Total returned records | 1..1        | Extension-CPIS-TotalRecords.valuePositiveInt | This count will be carried in {{pagelink:ExtensionCPIS-TotalRecords}}.                                                                                                                        |
|                        | 1..1        | status                                       | Fixed value = <code>current</code>.                                                                                                                                                           |
|                        | 1..1        | mode                                         | Fixed value = <code>snapshot</code>.                                                                                                                                                          |
|                        | 1..1        | code                                         | Code.coding.system will be fixed to <code>http://snomed.info/sct</code>.<br>Code.coding.code will be fixed to <code>722160009</code>.<br>Code.coding.display will be fixed to <code>Audit trail report</code>. |
|                        | 0..1        | subject                                      | This element may reference {{pagelink:Patient}}.                                                                                                                                              |
|                        | 1..*        | entry.item                                   | This element will reference {{pagelink:AuditEvent}}.                                                                                                                                           |

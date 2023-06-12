## CarePlan

The Child Protection Information Sharing implementation uses the StructureDefinition CarePlan profiled as UKCore-CarePlan:

## UKCore-CarePlan ##

<div class="tab">
  <button class="tablinks" onclick="openTab(event, 'Differential View')">Differential View</button>
  <button class="tablinks active" onclick="openTab(event, 'Hybrid View')">Hybrid View</button>
  <button class="tablinks" onclick="openTab(event, 'Snapshot View')">Snapshot View</button>
  <button class="tablinks" onclick="openTab(event, 'Examples')">Examples</button>
</div>

<div id="Differential View" class="tabcontent">
  <h3>Differential View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-CarePlan, diff}}
</div>

<div id="Hybrid View" class="tabcontent" style="display:block">
  <h3>Hybrid View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-CarePlan, hybrid}}
</div>

<div id="Snapshot View" class="tabcontent">
  <h3>Snapshot View</h3>
 {{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-CarePlan, snapshot}}
</div>

<div id="Examples" class="tabcontent">
  <h3>Examples</h3>
There are currently no specific CP-IS examples for CarePlan. 

</div>



 ## Conformance Rules   

| Source data item | Cardinality | Target FHIR element | Conformance rules                                                                   |
|------------------|-------------|---------------------|-------------------------------------------------------------------------------------|
|                  | 1..1        | status              | A value will be selected from ValueSet [RequestStatus](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/82613) |
|                  | 1..1        | intent              | Fixed value = <code>plan</code>                                                                  |
| Plan type        | 1..1        | category            | A value will be selected from {{pagelink:ValueSetCPIS-PlanType}}. <br>Category.coding.system will be fixed to <code>https://fhir.nhs.uk/R4/ValueSet/CPIS-PlanType</code>.                                                                    |
| Start date       | 1..1        | period.start        |                                                                                     |
| End date         | 1..1        | period.end          |                                                                                     |
|                  | 1..1        | subject             | This element will reference the {{pagelink:Patient}} resource as the subject of the care plan.                                           |
|                  | 1..1        | author              | This element will reference the {{pagelink:Organization}} resource as the record submitter.                                         |
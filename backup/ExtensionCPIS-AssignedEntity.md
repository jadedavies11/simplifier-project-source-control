## Extension CPIS-AssignedEntity

This extension extends the Device resource to carry a reference to the PractitionerRole resource as the assigned entity for a device.

## Context of Use 
The following contexts of use have been applied to this Extension:

|type|expression|
|--
|resource|Device|

<div class="tab">
  <button class="tablinks active" onclick="openTab(event, 'Differential View')">Differential View</button>
  <button class="tablinks" onclick="openTab(event, 'Hybrid View')">Hybrid View</button>
  <button class="tablinks" onclick="openTab(event, 'Snapshot View')">Snapshot View</button>
  <button class="tablinks" onclick="openTab(event, 'Examples')">Examples</button>
</div>

<div id="Differential View" class="tabcontent" style="display:block">
  <h3>Differential View</h3>
{{tree:https://fhir.nhs.uk/R4/StructureDefinition/Extension-CPIS-AssignedEntity, diff}}
</div>

<div id="Hybrid View" class="tabcontent">
  <h3>Hybrid View</h3>
{{tree:https://fhir.nhs.uk/R4/StructureDefinition/Extension-CPIS-AssignedEntity, hybrid}}
</div>

<div id="Snapshot View" class="tabcontent">
  <h3>Snapshot View</h3>
 {{tree:https://fhir.nhs.uk/R4/StructureDefinition/Extension-CPIS-AssignedEntity, snapshot}}
</div>


<div id="Examples" class="tabcontent">
  <h3>Examples</h3>
There are currently no specific CP-IS examples for this extension. 

</div>

## Conformance Rules   

| Source data item | Cardinality | Target FHIR element                       | Conformance rules                                                  |
|------------------|-------------|-------------------------------------------|--------------------------------------------------------------------|
| Assigned entity  | 1..1        | valueReference (UK Core PractitionerRole) | This is a reference to the {{pagelink:PractitionerRole}} resource. |
## Extension CPIS-TotalRecords

This extension extends the List resource to support the exchange of total returned records for an NHS Query response for a specified NHS number.

## Context of Use 
The following contexts of use have been applied to this Extension:

|type|expression|
|--
|resource|List|

<div class="tab">
  <button class="tablinks active" onclick="openTab(event, 'Differential View')">Differential View</button>
  <button class="tablinks" onclick="openTab(event, 'Hybrid View')">Hybrid View</button>
  <button class="tablinks" onclick="openTab(event, 'Snapshot View')">Snapshot View</button>
  <button class="tablinks" onclick="openTab(event, 'Examples')">Examples</button>
</div>

<div id="Differential View" class="tabcontent" style="display:block">
  <h3>Differential View</h3>
{{tree:https://fhir.nhs.uk/R4/StructureDefinition/Extension-CPIS-TotalRecords, diff}}
</div>

<div id="Hybrid View" class="tabcontent">
  <h3>Hybrid View</h3>
{{tree:https://fhir.nhs.uk/R4/StructureDefinition/Extension-CPIS-TotalRecords, hybrid}}
</div>

<div id="Snapshot View" class="tabcontent">
  <h3>Snapshot View</h3>
 {{tree:https://fhir.nhs.uk/R4/StructureDefinition/Extension-CPIS-TotalRecords, snapshot}}
</div>


<div id="Examples" class="tabcontent">
  <h3>Examples</h3>
There are currently no specific CP-IS examples for this extension. 

</div>

## Conformance Rules

| Source data item       | Cardinality | Target FHIR element | Conformance rules                                                            |
|------------------------|-------------|---------------------|------------------------------------------------------------------------------|
| Total returned records | 1..1        | valuepositiveInt    | This element carries a count of the returned records for a given NHS number. |
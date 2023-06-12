## Practitioner

The Child Protection Information Sharing implementation uses the StructureDefinition Practitioner profiled as UKCore-Practitioner:

## UKCore-Practitioner ##

<div class="tab">
  <button class="tablinks" onclick="openTab(event, 'Differential View')">Differential View</button>
  <button class="tablinks active" onclick="openTab(event, 'Hybrid View')">Hybrid View</button>
  <button class="tablinks" onclick="openTab(event, 'Snapshot View')">Snapshot View</button>
  <button class="tablinks" onclick="openTab(event, 'Examples')">Examples</button>
</div>

<div id="Differential View" class="tabcontent">
  <h3>Differential View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-Practitioner, diff}}
</div>

<div id="Hybrid View" class="tabcontent" style="display:block">
  <h3>Hybrid View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-Practitioner, hybrid}}
</div>

<div id="Snapshot View" class="tabcontent">
  <h3>Snapshot View</h3>
 {{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-Practitioner, snapshot}}
</div>

<div id="Examples" class="tabcontent">
  <h3>Examples</h3>
There are currently no specific CP-IS examples for PractitionerRole. 

</div>

 ## Conformance Rules

 For an Author person:   

| Source data item | Cardinality | Target FHIR element        | Conformance rules                                                                                                                                                                                                                                    |
|------------------|-------------|----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| SDS user ID      | 0..1        | identifier:sdsUserID.value | Practitioner.identifier.system will be fixed to <code>https://fhir.nhs.uk/Id/sds-user-id</code>.<br> The value will be an SDS user ID.                                                                                                               |
| Use              | 0..1        | name.use                   | The FHIR R4 selected value will be either <code>usual</code> or <code>nickname</code>.<br>[Mappings are provided](https://simplifier.net/guide/ChildProtection/ConceptMaps) to the CP-IS HL7 V3 values of <code>L</code> and <code>PREFERRED</code>. |
| Family name      | 1..1        | name.family                |                                                                                                                                                                                                                                                      |
| Given name       | 1..*        | name.given                 |                                                                                                                                                                                                                                                      |
| Prefix           | 1..1        | name.prefix                |                                                                                                                                                                                                                                                      |
| Suffix           | 0..1        | name.suffix                |                                                                                                                                                                                                                                                      |
| ValidTime.start  | 0..1        | period.start               |                                                                                                                                                                                                                                                      |
| ValidTime.end    | 0..1        | period.end                 |                                                                                                                                                                                                                                                      |

For an Author device:

| Source data item | Cardinality | Target FHIR element | Conformance rules                                                                                                                                                                                                                                    |
|------------------|-------------|---------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Use              | 0..1        | name.use            | The FHIR R4 selected value will be either <code>usual</code> or <code>nickname</code>.<br>[Mappings are provided](https://simplifier.net/guide/ChildProtection/ConceptMaps) to the CP-IS HL7 V3 values of <code>L</code> and <code>PREFERRED</code>. |
| Family name      | 1..1        | name.family         |                                                                                                                                                                                                                                                      |
| Given name       | 1..*        | name.given          |                                                                                                                                                                                                                                                      |
| Prefix           | 1..1        | name.prefix         |                                                                                                                                                                                                                                                      |
| Suffix           | 0..1        | name.suffix         |                                                                                                                                                                                                                                                      |
| ValidTime.start  | 0..1        | period.start        |                                                                                                                                                                                                                                                      |
| ValidTime.end    | 0..1        | period.end          |                                                                                                                                                                                                                                                      |
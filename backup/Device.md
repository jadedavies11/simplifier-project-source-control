## Device

The Child Protection Information Sharing implementation uses the StructureDefinition Device profiled as UKCore-Device:

## UKCore-Device ##

<div class="tab">
  <button class="tablinks" onclick="openTab(event, 'Differential View')">Differential View</button>
  <button class="tablinks active" onclick="openTab(event, 'Hybrid View')">Hybrid View</button>
  <button class="tablinks" onclick="openTab(event, 'Snapshot View')">Snapshot View</button>
  <button class="tablinks" onclick="openTab(event, 'Examples')">Examples</button>
</div>

<div id="Differential View" class="tabcontent">
  <h3>Differential View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-Device, diff}}
</div>

<div id="Hybrid View" class="tabcontent" style="display:block">
  <h3>Hybrid View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-Device, hybrid}}
</div>

<div id="Snapshot View" class="tabcontent">
  <h3>Snapshot View</h3>
 {{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-Device, snapshot}}
</div>

<div id="Examples" class="tabcontent">
  <h3>Examples</h3>
There are no specific CP-IS examples for Device. 

</div>


 ## Conformance Rules   

| Source data item                   | Cardinality | Target FHIR element                                                                                        | Conformance rules                                                                                                                                                                                                                                                                                       |
|------------------------------------|-------------|------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Job role code (person responsible) | 1..1        | UK Core Device.Extension-CPIS-AssignedEntity (UK Core PractitionerRole).code:sdsJobRoleName.coding.code    | A value will be selected from the ValueSet [UKCoreSDSJobRoleName](https://simplifier.net/packages/uk.core.r4.v2/2.0.8/files/322975).<br>UK Core PractitionerRole.code:sdsJobRoleName.coding.system will be fixed to <code>https://fhir.hl7.org.uk/CodeSystem/UKCore-SDSJobRoleName</code>.<br>Note that the extension has a cardinality of 0..* within its extended resource. |
| Job role name (person responsible) | 1..1        | UK Core Device.Extension-CPIS-AssignedEntity (UK Core PractitionerRole).code:sdsJobRoleName.coding.display | This will be the display name for the code chosen.                                                                                                                                                                                                                                                      |
| Identifier                         | 1..1        | identifier.value                                                                            | Identifier.system will be fixed to <code>https://fhir.nhs.uk/Id/nhsSpineASID</code>.                                                                                                                                                                                                                      |
| Organisation identifier            | 1..1        |  owner.identifier.value                                                                      | This element will carry the identifier (ODS organisation or Site code) of the organisation which owns the device.<br>Owner.identifier.system will be fixed to <code>https://fhir.nhs.uk/Id/ods-organization-code</code> or <code>https://fhir.nhs.uk/Id/ods-site-code</code>.                         |
| Organisation name                  | 1..1        | owner.display                                                                               | This element will carry the name of the organisation which owns the device.                                                                                                                                                                                                                             |
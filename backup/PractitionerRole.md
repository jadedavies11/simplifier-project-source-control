## PractitionerRole

The Child Protection Information Sharing implementation uses the StructureDefinition PractitionerRole profiled as UKCore-PractitionerRole:

## UKCore-PractitionerRole ##

<div class="tab">
  <button class="tablinks" onclick="openTab(event, 'Differential View')">Differential View</button>
  <button class="tablinks active" onclick="openTab(event, 'Hybrid View')">Hybrid View</button>
  <button class="tablinks" onclick="openTab(event, 'Snapshot View')">Snapshot View</button>
  <button class="tablinks" onclick="openTab(event, 'Examples')">Examples</button>
</div>

<div id="Differential View" class="tabcontent">
  <h3>Differential View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-PractitionerRole, diff}}
</div>

<div id="Hybrid View" class="tabcontent" style="display:block">
  <h3>Hybrid View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-PractitionerRole, hybrid}}
</div>

<div id="Snapshot View" class="tabcontent">
  <h3>Snapshot View</h3>
 {{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-PractitionerRole, snapshot}}
</div>

<div id="Examples" class="tabcontent">
  <h3>Examples</h3>
There are currently no specific CP-IS examples for PractitionerRole. 

</div>

 ## Conformance Rules

 For an Author person:   

| Source data item | Cardinality | Target FHIR element                 | Conformance rules                                                                                                                                                                                                                                                                          |
|------------------|-------------|-------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|                  | 0..1        | identifier:sdsRoleProfileID.value   | PractitionerRole.identifier.system will be fixed to <code>https://fhir.nhs.uk/Id/sds-role-profile-id</code>.<br> The value will be an SDS role profile ID.                                                                                                                                 |
|                  | 1..1        | practitioner (UK Core Practitioner) | This element will reference the {{pagelink:Practitioner}} resource.                                                                                                                                                                                                                        |
|                  | 1..1        | organization (UK Core Organization) | This element will reference the {{pagelink:Organization}} resource.                                                                                                                                                                                                                        |
| Job role code    | 1..1        | code:sdsJobRoleName.coding.code     | A value will be selected from the ValueSet [UKCoreSDSJobRoleName](https://simplifier.net/packages/uk.core.r4.v2/2.0.8/files/322975).<br>UK Core PractitionerRole.code:sdsJobRoleName.coding.system will be fixed to <code>https://fhir.hl7.org.uk/CodeSystem/UKCore-SDSJobRoleName</code>. |
| Job role name    | 1..1        | code.sdsJobRoleName.coding.display  | This will be the display name for the code chosen                                                                                                                                                                                                                                          |

For an Author device:

| Source data item | Cardinality | Target FHIR element                 | Conformance rules                                                                                                                                                                                                                                                                          |
|------------------|-------------|-------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|                  | 1..1        | practitioner (UK Core Practitioner) | This element will reference the {{pagelink:Practitioner}} resource.                                                                                                                                                                                                                        |
| Job role code    | 1..1        | code:sdsJobRoleName.coding.code     | A value will be selected from the ValueSet [UKCoreSDSJobRoleName](https://simplifier.net/packages/uk.core.r4.v2/2.0.8/files/322975).<br>UK Core PractitionerRole.code:sdsJobRoleName.coding.system will be fixed to <code>https://fhir.hl7.org.uk/CodeSystem/UKCore-SDSJobRoleName</code>. |
| Job role name    | 1..1        | code.sdsJobRoleName.coding.display  | This will be the display name for the code chosen                                                                                                                                                                                                                                          |
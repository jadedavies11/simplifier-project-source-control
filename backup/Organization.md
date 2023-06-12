## Organization

The Child Protection Information Sharing implementation uses the StructureDefinition Organization profiled as UKCore-Organization:

## UKCore-Organization ##

<div class="tab">
  <button class="tablinks" onclick="openTab(event, 'Differential View')">Differential View</button>
  <button class="tablinks active" onclick="openTab(event, 'Hybrid View')">Hybrid View</button>
  <button class="tablinks" onclick="openTab(event, 'Snapshot View')">Snapshot View</button>
  <button class="tablinks" onclick="openTab(event, 'Examples')">Examples</button>
</div>

<div id="Differential View" class="tabcontent">
  <h3>Differential View</h3>
{{tree:uk.core.r4.v2@2.0.8/package/UKCore-Organization.json, diff}}
</div>

<div id="Hybrid View" class="tabcontent" style="display:block">
  <h3>Hybrid View</h3>
{{tree:uk.core.r4.v2@2.0.8/package/UKCore-Organization.json, hybrid}}
</div>

<div id="Snapshot View" class="tabcontent">
  <h3>Snapshot View</h3>
{{tree:uk.core.r4.v2@2.0.8/package/UKCore-Organization.json, snapshot}}
</div>

<div id="Examples" class="tabcontent">
  <h3>Examples</h3>
There are currently no specific CP-IS examples for Organization. 

</div>

# Conformance Rules

All organisations represented in CP-IS will have an identifier and a name as below:-

| Source data item                          | Cardinality | Target FHIR element                                                  | Conformance rules                                                                                                                                                                                                                                                                                                                                                 |
|-------------------------------------------|-------------|----------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Organisation identifier                   | 1..1        | identifier:odsOrganisationCode.value or identifier:odsSiteCode.value | Organisation.identifier.system will be fixed to <code>https://fhir.nhs.uk/Id/ods-organization-code</code> or <code>https://fhir.nhs.uk/Id/ods-site-code</code>.<br> The value will be an ODS organisation or site code.                                                                                                                                                                 |
| Organisation name                         | 1..1        | name                                                                 | The corresponding ODS name of the organisation or site.                                                                                                                                                                                                                                                                                                                         |

The organisation which authored a care plan will additionally have the following elements:-

| Source data item                          | Cardinality | Target FHIR element         | Conformance rules                                                                                                                                                                                                                                                                                                                                                 |
|-------------------------------------------|-------------|-----------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Organisation telephone number (Emergency) | 1..1        | telecom.value               | Telecom.system will be fixed to <code>phone</code>.                                                                                                                                                                                                                                                                                                     |
| Organisation telephone number use         | 1..1        | contact.purpose.coding.code | Contact.purpose.coding.system will be fixed to  <code>http://terminology.hl7.org/CodeSystem/v3-AddressUse</code>.<br> Contact.purpose.coding.code will be fixed to <code>EC</code>.<br>Contact.purpose.coding.display will be fixed to  <code>emergency contact</code>.<br>The telecom.use value will be selected from the ValueSet [ContactPointUse](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/80239). |
| Organisation telephone number (Workplace) | 0..1        | telecom.value               | Telecom.system will be fixed to <code>phone</code>.                                                                                                                                                                                                                                                                                                     |
| Organisation telephone number use         | 0..1        | contact.purpose.coding.code | Contact.purpose.coding.system will be fixed to <code>http://terminology.hl7.org/CodeSystem/v3-AddressUse</code>.<br> Contact.purpose.coding.code will be fixed to <code>WP</code>.<br>Contact.purpose.coding.display will be fixed to <code>work place</code>.<br> The telecom.use value will be selected from the ValueSet [ContactPointUse](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/80239).        |
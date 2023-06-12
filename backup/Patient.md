## Patient

The Child Protection Information Sharing implementation uses the StructureDefinition Patie profiled as UKCore-Patient:

## UKCore-Patient ##

<div class="tab">
  <button class="tablinks" onclick="openTab(event, 'Differential View')">Differential View</button>
  <button class="tablinks active" onclick="openTab(event, 'Hybrid View')">Hybrid View</button>
  <button class="tablinks" onclick="openTab(event, 'Snapshot View')">Snapshot View</button>
  <button class="tablinks" onclick="openTab(event, 'Examples')">Examples</button>
</div>

<div id="Differential View" class="tabcontent">
  <h3>Differential View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-Patient, diff}}
</div>

<div id="Hybrid View" class="tabcontent" style="display:block">
  <h3>Hybrid View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-Patient, hybrid}}
</div>

<div id="Snapshot View" class="tabcontent">
  <h3>Snapshot View</h3>
 {{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-Patient, snapshot}}
</div>

<div id="Examples" class="tabcontent">
  <h3>Examples</h3>
There are currently no specific CP-IS examples for Patient. 

</div>



 ## Conformance Rules   

| Source data item | Cardinality | Target FHIR element                          | Conformance rules                                                                                                                                                                                                                                              |
|------------------|-------------|----------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| NHS number       | 1..1        | identifier (nhsNumber)       |                                                                                                                                                                                                                                                                |
|                  | 1..1        | Extension-UKCore-NHSNumberVerificationStatus | A value will be selected from ValueSet [UKCoreNHSNumberVerificationStatus](https://simplifier.net/packages/uk.core.r4.v2/2.0.8/files/323043).<br>Extension-UKCore-NHSNumberVerificationStatus.valueCodeableConcept.system will be fixed to <code>https://fhir.hl7.org.uk/CodeSystem/UKCore-NHSNumberVerificationStatus</code>. |
| Local identifier | 0..1        | identifier.value             | This element may be populated by a locally assigned identifier.                                                                                                                                                                                                 |
| Family name      | 1..1        | name.family                  |                                                                                                                                                                                                                                                                |
| Given name       | 1..*        | name.given                   |                                                                                                                                                                                                                                                                |
| Date of birth    | 1..1        | birthDate                    | This element will have the extension [birthTime](http://hl7.org/fhir/extension-patient-birthtime.html) to carry the time of birth.                                                                                                                             |
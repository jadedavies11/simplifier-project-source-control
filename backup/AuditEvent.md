## AuditEvent

The Child Protection Information Sharing implementation uses the StructureDefinition AuditEvent profiled as UKCore-AuditEvent:

## UKCore-AuditEvent ##

<div class="tab">
  <button class="tablinks" onclick="openTab(event, 'Differential View')">Differential View</button>
  <button class="tablinks active" onclick="openTab(event, 'Hybrid View')">Hybrid View</button>
  <button class="tablinks" onclick="openTab(event, 'Snapshot View')">Snapshot View</button>
  <button class="tablinks" onclick="openTab(event, 'Examples')">Examples</button>
</div>

<div id="Differential View" class="tabcontent">
  <h3>Differential View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-AuditEvent, diff}}
</div>

<div id="Hybrid View" class="tabcontent" style="display:block">
  <h3>Hybrid View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-AuditEvent, hybrid}}
</div>

<div id="Snapshot View" class="tabcontent">
  <h3>Snapshot View</h3>
 {{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-AuditEvent, snapshot}}
</div>

<div id="Examples" class="tabcontent">
  <h3>Examples</h3>
There are currently no specific CP-IS examples for AuditEvent. 

</div>



 ## Conformance Rules

| Source data item | Cardinality | Target FHIR element                  | Conformance rules                                                                                                                                                                                                                                          |
|------------------|-------------|--------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|                  | 1..1        | type                                 | A value will be selected from the ValueSet [AuditEventID](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/81250).                                                                                                                             |
| Effective time   | 1..1        | recorded                             |                                                                                                                                                                                                                                                            |
| Author device    | 0..1        | agent.who (UK Core Device)           | This element will reference {{pagelink:Device}}.                                                                                                                                                                                                           |
| Author person    | 0..1        | agent.who (UK Core PractitionerRole) | This element will reference {{pagelink:PractitionerRole}}.                                                                                                                                                                                                 |
|                  | 0..*        | agent.role                           | Agent.role.coding.system will be fixed to <code>https://www.hl7.org/fhir/v3/ParticipationType/cs.html</code>.<br>Agent.role.coding.code will be fixed to <code>AUT</code>.<br>Agent.role.coding.display will be fixed to <code>author (originator)</code>. |
|                  | 1..1        | agent.requestor                      | This element will be fixed to <code>true</code>.                                                                                                                                                                                                           |
|                  | 1..1        | source.observer                      | This element will reference [Device](https://simplifier.net/guide/ChildProtection/Device) for an author device.<br>This will reference [PractitionerRole](https://simplifier.net/guide/ChildProtection/PractitionerRole) for an author person.             |
|                  | 0..1        | entity.what                          | This element will reference {{pagelink:Patient}}.                                                                                                                                                                                                          |
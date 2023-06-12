## Bundle

The Child Protection Information Sharing implementation uses the StructureDefinition Bundle profiled as UKCore-Bundle:

## UKCore-Bundle ##

<div class="tab">
  <button class="tablinks" onclick="openTab(event, 'Differential View')">Differential View</button>
  <button class="tablinks active" onclick="openTab(event, 'Hybrid View')">Hybrid View</button>
  <button class="tablinks" onclick="openTab(event, 'Snapshot View')">Snapshot View</button>
  <button class="tablinks" onclick="openTab(event, 'Examples')">Examples</button>
</div>

<div id="Differential View" class="tabcontent">
  <h3>Differential View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-Bundle, diff}}
</div>

<div id="Hybrid View" class="tabcontent" style="display:block">
  <h3>Hybrid View</h3>
{{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-Bundle, hybrid}}
</div>

<div id="Snapshot View" class="tabcontent">
  <h3>Snapshot View</h3>
 {{tree:https://fhir.hl7.org.uk/StructureDefinition/UKCore-Bundle, snapshot}}
</div>

<div id="Examples" class="tabcontent">
  <h3>Examples</h3>

</br>
{{pagelink:ExampleCPISBundle}}

</div>



 ## Conformance Rules   
 
Source Data Item | Cardinality | Target FHIR Element | Conformance rules |
|--
|EffectiveTime|1..1|timestamp||
||1..1|type|Fixed value = <code>searchset</code>|
||1..*|entry.resource|This element will carry the resources which are entries in the bundle.|
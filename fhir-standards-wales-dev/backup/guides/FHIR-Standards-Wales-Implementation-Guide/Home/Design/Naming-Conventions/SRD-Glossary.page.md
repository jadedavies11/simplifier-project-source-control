<table class="table table-striped">
	<thead>
		<tr>
			<th scope="col"><b>Term</b></th>
			<th scope="col"><b>Definition</b></th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td scope="row"><b>DataStandardsWales</b></td>
			<td>This fixed value indicates that this is a Wales-wide standard, equally applicable to exchange or storage of FHIR data in any system in Wales.</td>
		</tr>	
		<tr>
			<td scope="row"><b><span style="color:#c00000;">BusinessName</span></b></td>
			<td>The business name of the resource. Constructed according to rules specific to the resource type.  UpperCamelCase used for each contributing element.</td>
		</tr>	
		<tr>
			<td scope="row"><b><span style="color:#0070c0;">Discriminator</span></b></td>
			<td>This is used to distinguish one FHIR asset type from another. It is typically the Level 2 HL7 resource type such as CodeSystem, but it is also used to distinguish Profile from Extension as both are instances of the StructureDefinition resource type.</td>
		</tr>
		<tr>
			<td scope="row">.xml</td>
			<td>Resources are defined using xml to ensure that the correct element order is made explicit for resource instances created using xml. The json equivalent is published via conversion from xml in the implementation guide.</td>
		</tr>	
		<tr>
			<td scope="row"><b>baseUrl</b></td>
			<td>This fixed value of <b>https://fhir.nhs.wales</b> applies to all resource definitions in the Wales FHIR Implementation Guide.</td>
		</tr>	
		<tr>
			<td scope="row"><b><span style="color:#ff9900;">L2ResourceType</span></b></td>
			<td><a href="https://hl7.org/fhir/R4/" target="_blank">The Level 2 FHIR resource type.</a> The resource definitions covered by this section are of the following types: StructureDefinition, MessageDefinition, CodeSystem and ValueSet. ConceptMap and NamingSystem definitions are covered separately in the “Additional naming conventions” section  below.</td>
		</tr>	
		<tr>
			<td scope="row"><b><span style="color:#9c7406;">L3L4ResourceType</span></b></td>
			<td><a href="https://hl7.org/fhir/R4/" target="_blank">The Level 3 or Level 4 resource type</a> e.g.‘Patient’, ‘Organization’, ‘Observation’, ‘Medication’.</td>
		</tr>	
		<tr>
			<td scope="row"><b><span style="color:#c00000;">Descriptor</span></b></td>
			<td>A simple descriptor for the subject of the resource definition. For CodeSystem and ValueSet, where applicable, this shall reflect the name given to the data set as published in the relevant Data Standards Change Notice (DSCN). For ConceptMap resources, this shall reflect the name given to the value set that is being mapped to or from.</td>
		</tr>
		<tr>
			<td scope="row"><b><span style="color:#c00000;">MessageEvent</span></b></td>
			<td>The code for the message event, converted from kebab-case to UpperCamelCase.</td>
		</tr>
		<tr>
			<td scope="row"><b><span style="color:#7030a0;">Qualifier</span></b></td>
			<td>Used as an additional descriptor when existing resources are specialised for a specific use case.</td>
		</tr>
    </tbody>
</table>

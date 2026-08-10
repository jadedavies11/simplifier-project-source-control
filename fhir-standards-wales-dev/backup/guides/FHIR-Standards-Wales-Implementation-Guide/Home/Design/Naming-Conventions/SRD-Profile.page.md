<b>Filename structure:</b> <span style="color:#0070c0;">Profile-</span>DataStandardsWales-<span style="color:#914829;">[L3L4ResourceType]</span><span style="color:#7030a0;">{-[Qualifier]}{-[Qualifier]}​</span><br />
<b>id structure:</b> DataStandardsWales-<span style="color:#914829;">[L3L4ResourceType]</span><span style="color:#7030a0;">{-[Qualifier]}{-[Qualifier]}​</span><br /><br />
​
<i>Note that in line with UK and international practice the “Profile” discriminator is omitted from id and name and from uses derived from those elements.​</i><br /><br />
​
<b><i>Worked example 1 (profile)​</i></b><br />
<span style="font-size: 0.9em;">A profile to apply Wales-specific standards to the UKCore-Observation profile.  The optional qualifier component is not applicable in this case.</span>

<table class="table properties-table">
	<tbody>
		<tr>
			<th scope="row">Asset filename</th>
			<td>Profile-DataStandardsWales-Observation.xml</td>
		</tr>
		<tr>
			<th scope="row">Page filename</th>
			<td>Profile-DataStandardsWales-Observation.page.md</td>
		</tr>
		<tr>
			<th scope="row">id</th>
			<td>DataStandardsWales-Observation</td>
		</tr>	
		<tr>
			<th scope="row">name</th>
			<td>DataStandardsWalesObservation</td>
		</tr>	
		<tr>
			<th scope="row">title</th>
			<td>Data Standards Wales Observation</td>
		</tr>	
		<tr>
			<th scope="row">url</th>
			<td>https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Observation</td>
		</tr>	
		<tr>
			<th scope="row">reference</th>
			<td>StructureDefinition/DataStandardsWales-Observation</td>
		</tr>
    </tbody>
</table>

<b><i>Worked example 2 (sub-profile)​</i></b><br />
<span style="font-size: 0.9em;">A profile to specialize the DataStandardsWales-Observation profile for the capture of vital signs observations.</span>

<table class="table properties-table">
	<tbody>
		<tr>
			<th scope="row">Asset filename</th>
			<td>Profile-DataStandardsWales-Observation-VitalSigns.xml</td>
		</tr>
		<tr>
			<th scope="row">Page filename</th>
			<td>Profile-DataStandardsWales-Observation-VitalSigns.page.md</td>
		</tr>
		<tr>
			<th scope="row">id</th>
			<td>DataStandardsWales-Observation-VitalSigns</td>
		</tr>	
		<tr>
			<th scope="row">name</th>
			<td>DataStandardsWalesObservationVitalSigns</td>
		</tr>	
		<tr>
			<th scope="row">title</th>
			<td>Data Standards Wales Observation Vital Signs</td>
		</tr>	
		<tr>
			<th scope="row">url</th>
			<td>https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Observation-VitalSigns</td>
		</tr>	
		<tr>
			<th scope="row">reference</th>
			<td>StructureDefinition/DataStandardsWales-Observation-VitalSigns</td>
		</tr>
    </tbody>
</table>	

<b><i>Worked example 3 (sub-profile)​</i></b><br />
<span style="font-size: 0.9em;">A profile to specialize the DataStandardsWales-Observation-VitalSigns profile for the capture of BMI.</span>

<table class="table properties-table">
	<tbody>
		<tr>
			<th scope="row">Asset filename</th>
			<td>Profile-DataStandardsWales-Observation-VitalSigns-BMI.xml</td>
		</tr>
		<tr>
			<th scope="row">Page filename</th>
			<td>Profile-DataStandardsWales-Observation-VitalSigns-BMI.page.md</td>
		</tr>
		<tr>
			<th scope="row">id</th>
			<td>DataStandardsWales-Observation-VitalSigns-BMI</td>
		</tr>	
		<tr>
			<th scope="row">name</th>
			<td>DataStandardsWalesObservationVitalSignsBMI</td>
		</tr>	
		<tr>
			<th scope="row">title</th>
			<td>Data Standards Wales Observation Vital Signs BMI</td>
		</tr>	
		<tr>
			<th scope="row">url</th>
			<td>https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Observation-VitalSigns-BMI</td>
		</tr>	
		<tr>
			<th scope="row">reference</th>
			<td>StructureDefinition/DataStandardsWales-Observation-VitalSigns-BMI</td>
		</tr>
    </tbody>
</table>
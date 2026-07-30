<b>Filename structure:</b> <span style="color:#0070c0;">Profile-</span>DataStandardsWales-<span style="color:#9c7406;">[L3L4ResourceType]</span><span style="color:#7030a0;">{-[Qualifier]}{-[Qualifier]}​</span><br />
<b>id structure:</b> DataStandardsWales-<span style="color:#9c7406;">[L3L4ResourceType]</span><span style="color:#7030a0;">{-[Qualifier]}{-[Qualifier]}​</span><br /><br />
​
<i>Note that in line with UK and international practice the “Profile” discriminator is omitted from id and name and from uses derived from those elements.​</i><br /><br />
​
<b><i>Worked example 1 (profile)​</i></b><br />
A profile to apply Wales-specific standards to the UKCore-Observation profile.  The optional qualifier component is not applicable in this case.

<table class="table table-striped">
	<thead>
		<tr>
			<th scope="col"><b>Element</b></th>
			<th scope="col"><b>Example</b></th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td scope="row">Asset filename</td>
			<td>Profile-DataStandardsWales-Observation.xml</td>
		</tr>
		<tr>
			<td scope="row">Page filename</td>
			<td>Profile-DataStandardsWales-Observation.page.md</td>
		</tr>
		<tr>
			<td scope="row">id</td>
			<td>DataStandardsWales-Observation</td>
		</tr>	
		<tr>
			<td scope="row">name</td>
			<td>DataStandardsWalesObservation</td>
		</tr>	
		<tr>
			<td scope="row">title</td>
			<td>Data Standards Wales Observation</td>
		</tr>	
		<tr>
			<td scope="row">url</td>
			<td>https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Observation</td>
		</tr>	
		<tr>
			<td scope="row">reference</td>
			<td>StructureDefinition/DataStandardsWales-Observation</td>
		</tr>
    </tbody>
</table>

<b><i>Worked example 2 (sub-profile)​</i></b><br />
A profile to specialize the DataStandardsWales-Observation profile for the capture of vital signs observations.

<table class="table table-striped">
	<thead>
		<tr>
			<th scope="col"><b>Element</b></th>
			<th scope="col"><b>Example</b></th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td scope="row">Asset filename</td>
			<td>Profile-DataStandardsWales-Observation-VitalSigns.xml</td>
		</tr>
		<tr>
			<td scope="row">Page filename</td>
			<td>Profile-DataStandardsWales-Observation-VitalSigns.page.md</td>
		</tr>
		<tr>
			<td scope="row">id</td>
			<td>DataStandardsWales-Observation-VitalSigns</td>
		</tr>	
		<tr>
			<td scope="row">name</td>
			<td>DataStandardsWalesObservationVitalSigns</td>
		</tr>	
		<tr>
			<td scope="row">title</td>
			<td>Data Standards Wales Observation Vital Signs</td>
		</tr>	
		<tr>
			<td scope="row">url</td>
			<td>https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Observation-VitalSigns</td>
		</tr>	
		<tr>
			<td scope="row">reference</td>
			<td>StructureDefinition/DataStandardsWales-Observation-VitalSigns</td>
		</tr>
    </tbody>
</table>	

<b><i>Worked example 3 (sub-profile)​</i></b><br />
A profile to specialize the DataStandardsWales-Observation-VitalSigns profile for the capture of BMI.

<table class="table table-striped">
	<thead>
		<tr>
			<th scope="col"><b>Element</b></th>
			<th scope="col"><b>Example</b></th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td scope="row">Asset filename</td>
			<td>Profile-DataStandardsWales-Observation-VitalSigns-BMI.xml</td>
		</tr>
		<tr>
			<td scope="row">Page filename</td>
			<td>Profile-DataStandardsWales-Observation-VitalSigns-BMI.page.md</td>
		</tr>
		<tr>
			<td scope="row">id</td>
			<td>DataStandardsWales-Observation-VitalSigns-BMI</td>
		</tr>	
		<tr>
			<td scope="row">name</td>
			<td>DataStandardsWalesObservationVitalSignsBMI</td>
		</tr>	
		<tr>
			<td scope="row">title</td>
			<td>Data Standards Wales Observation Vital Signs BMI</td>
		</tr>	
		<tr>
			<td scope="row">url</td>
			<td>https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Observation-VitalSigns-BMI</td>
		</tr>	
		<tr>
			<td scope="row">reference</td>
			<td>StructureDefinition/DataStandardsWales-Observation-VitalSigns-BMI</td>
		</tr>
    </tbody>
</table>
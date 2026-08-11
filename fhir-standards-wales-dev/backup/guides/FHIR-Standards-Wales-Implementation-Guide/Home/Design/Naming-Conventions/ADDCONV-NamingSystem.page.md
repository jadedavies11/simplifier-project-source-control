<b>Filename structure:</b> <span style="color:#0070c0;">NamingSystem-</span><span style="color:#198248;">{[Organisation]}-{[System]}-</span><span style="color:#c00000;">[descriptor]</span><br />
<b>id structure:</b> DataStandardsWales-<span style="color:#198248;">{[Organisation]}-{[System]}-</span><span style="color:#c00000;">[Descriptor]</span><br />
<b>name structure:</b> <span style="color:#198248;">{[Organisation]}{[System]}</span><span style="color:#c00000;">[Descriptor]</span><br />
<b>uniqueId value structure:</b>https://fhir.[ownerdomain]/Id/<span style="color:#c00000;">[Descriptor]</span><br /><br />

The formal convention is for Descriptor to be consistent between id, name and uniqueId, but the influence of external owners means this is not always the case. There is variability by owning system and organisation, as illustrated by the examples below.​<br /><br />
​
<b><i>Worked example 1 - All Wales identifiers​</i></b><br />
<span style="font-size: 0.9em;">WRTS organization identifiers</span>

<table class="table properties-table">
	<tbody>
		<tr>
			<th scope="row">Asset filename</th>
			<td>NamingSystem-WRTS-organization-identifier.xml</td>
		</tr>
		<tr>
			<th scope="row">id</th>
			<td>DataStandardsWales-WRTS-OrganizationIdentifier</td>
		</tr>	
		<tr>
			<th scope="row">name</th>
			<td>WRTSOrganizationIdentifier</td>
		</tr>	
		<tr>
			<th scope="row">uniqueId</th>
			<td>https://fhir.nhs.wales/Id/wrts-organization-identifier</td>
		</tr>	
	</tbody>
</table>

<span style="font-size: 0.9em;">LIMS TCLe report identifiers</span>

<table class="table properties-table">
	<tbody>
		<tr>
			<th scope="row">Asset filename</th>
			<td>NamingSystem-LIMS-TCLe-report-identifier.xml</td>
		</tr>
		<tr>
			<th scope="row">id</th>
			<td>NHSWales-LIMS-TCLe-Report-Code</td>
		</tr>	
		<tr>
			<th scope="row">name</th>
			<td>TCLeReportCodeIdentifier</td>
		</tr>	
		<tr>
			<th scope="row">uniqueId</th>
			<td>https://fhir.nhs.wales/Id/lims-tcle-report-code</td>
		</tr>	
	</tbody>
</table>

<b><i>Worked example 2 - Identifiers issued by local PAS​</i></b><br />
<span style="font-size: 0.9em;">PAS Practitioner Identifier (CAVUHB)</span>

<table class="table properties-table">
	<tbody>
		<tr>
			<th scope="row">Asset filename</th>
			<td>NamingSystem-CAVUHB-pas-practitioner-identifier.xml</td>
		</tr>
		<tr>
			<th scope="row">id</th>
			<td>DataStandardsWales-CAVUHB-PAS-PractitionerIdentifier</td>
		</tr>	
		<tr>
			<th scope="row">name</th>
			<td>CAVUHBPASPractitionerIdentifier</td>
		</tr>	
		<tr>
			<th scope="row">uniqueId</th>
			<td>https://fhir.cavuhb.nhs.wales/Id/pas-practitioner-identifier</td>
		</tr>	
	</tbody>
</table>

<span style="font-size: 0.9em;">PAS Location Identifier (BCUHB)</span>

<table class="table properties-table">
	<tbody>
		<tr>
			<th scope="row">Asset filename</th>
			<td>NamingSystem-BCUHB-pas-location-identifier.xml</td>
		</tr>
		<tr>
			<th scope="row">id</th>
			<td>DataStandardsWales-BCUHB-PAS-LocationIdentifier</td>
		</tr>	
		<tr>
			<th scope="row">name</th>
			<td>BCUHBPASLocationIdentifier</td>
		</tr>	
		<tr>
			<th scope="row">uniqueId</th>
			<td>https://fhir.bcuhb.nhs.wales/Id/pas-location-identifier</td>
		</tr>	
	</tbody>
</table>
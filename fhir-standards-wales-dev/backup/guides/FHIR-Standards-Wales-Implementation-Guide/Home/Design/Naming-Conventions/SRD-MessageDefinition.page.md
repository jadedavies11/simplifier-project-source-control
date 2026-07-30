<b>Filename structure:</b> <span style="color:#0070c0;">MessageDefinition-</span>DataStandardsWales-<span style="color:#c00000;">[MessageEvent]</span><span style="color:#7030a0;">{-[Qualifier]}</span><br />
<b>id structure:</b> DataStandardsWales-<span style="color:#c00000;">[MessageEvent]</span><span style="color:#7030a0;">{-[Qualifier]}</span><br /><br />

<i>Note that typically each message event would have one corresponding message definition. However, the FHIR standard does allow for multiple MessageDefinition resources with the same message event code. In this case a qualifier should be used.</i>​<br /><br />
​
<b><i>Worked example​</i><br />
A message definition to submit a care document to a FHIR repository. The event code quoted will have been defined as part of a code system that is included in the bound DataStandardsWales-MessageEvent value set.

<table class="table table-striped">
	<thead>
		<tr>
			<th scope="col"><b>Element</b></th>
			<th scope="col"><b>Example</b></th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td scope="row">event.code</td>
			<td>care-document-submit</td>
		</tr>>
		<tr>
			<td scope="row">Asset filename</td>
			<td>MessageDefinition-DataStandardsWales-CareDocumentSubmit.xml</td>
		</tr>
		<tr>
			<td scope="row">Page filename</td>
			<td>MessageDefinition-DataStandardsWales-CareDocumentSubmit.page.md</td>
		</tr>
		<tr>
			<td scope="row">id</td>
			<td>DataStandardsWales-CareDocumentSubmit</td>
		</tr>	
		<tr>
			<td scope="row">name</td>
			<td>DataStandardsWalesCareDocumentSubmit</td>
		</tr>	
		<tr>
			<td scope="row">title</td>
			<td>Data Standards Wales Care Document Submit</td>
		</tr>	
		<tr>
			<td scope="row">url</td>
			<td>https://fhir.nhs.wales/MessageDefinition/DataStandardsWales-CareDocumentSubmit</td>
		</tr>	
		<tr>
			<td scope="row">reference</td>
			<td>MessageDefinition/DataStandardsWales-CareDocumentSubmit</td>
		</tr>
    </tbody>
</table>
<b>Filename structure:</b> <span style="color:#0070c0;">MessageDefinition-</span>DataStandardsWales-<span style="color:#c00000;">[MessageEvent]</span><span style="color:#7030a0;">{-[Qualifier]}</span><br />
<b>id structure:</b> DataStandardsWales-<span style="color:#c00000;">[MessageEvent]</span><span style="color:#7030a0;">{-[Qualifier]}</span><br /><br />

<i><span style="font-size: 0.9em;">Note that typically each message event would have one corresponding message definition. However, the FHIR standard does allow for multiple MessageDefinition resources with the same message event code. In this case a qualifier should be used.</span></i>​<br /><br />
​
<b><i>Worked example​</i></b><br />
<span style="font-size: 0.9em;">A message definition to submit a care document to a FHIR repository. The event code quoted will have been defined as part of a code system that is included in the bound DataStandardsWales-MessageEvent value set.</span>

<table class="table properties-table">
	<tbody>
		<tr>
			<th scope="row">event.code</th>
			<td>care-document-submit</td>
		</tr>
		<tr>
			<th scope="row">Asset filename</th>
			<td>MessageDefinition-DataStandardsWales-CareDocumentSubmit.xml</td>
		</tr>
		<tr>
			<th scope="row">Page filename</th>
			<td>MessageDefinition-DataStandardsWales-CareDocumentSubmit.page.md</td>
		</tr>
		<tr>
			<th scope="row">id</th>
			<td>DataStandardsWales-CareDocumentSubmit</td>
		</tr>	
		<tr>
			<th scope="row">name</th>
			<td>DataStandardsWalesCareDocumentSubmit</td>
		</tr>	
		<tr>
			<th scope="row">title</th>
			<td>Data Standards Wales Care Document Submit</td>
		</tr>	
		<tr>
			<th scope="row">url</th>
			<td>https://fhir.nhs.wales/MessageDefinition/DataStandardsWales-CareDocumentSubmit</td>
		</tr>	
		<tr>
			<th scope="row">reference</th>
			<td>MessageDefinition/DataStandardsWales-CareDocumentSubmit</td>
		</tr>
    </tbody>
</table>
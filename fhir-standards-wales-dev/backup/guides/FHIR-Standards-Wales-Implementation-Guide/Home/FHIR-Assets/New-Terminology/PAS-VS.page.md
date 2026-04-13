### {{page-title}}

The following ValueSets have been created for PAS use only.

<style>
  th, td {
    word-wrap: break-word;
    white-space: normal;
  }
</style>

<table class="table table-striped" style="table-layout: fixed;">
  <colgroup>
    <col style="width: 30%;">
    <col style="width: 30%;">
    <col style="width: 40%;">
  </colgroup>

  <thead>
    <tr>
      <th scope="col">ValueSet</th>
      <th scope="col">CodeSystem</th>
      <th scope="col">Additional information</th>
    </tr>
	</thead>
	<tbody>
	<tr>
		<td scope="row">{{pagelink:ValueSet-PASSourceAdmission, text: PASSourceAdmission}}</td>
		<td>{{pagelink:CodeSystem-WPASSourceAdmission, text: WPASSourceAdmission}}</td>
		<td>For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-PASReferralSource, text: PASReferralSource}}</td>
		<td>{{pagelink:CodeSystem-WPASReferralSource, text: WPASReferralSource}}<br>&<br>
		<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483937">UKCore-SourceOfServiceRequest</a>
		</td>
		<td>For CDR/ NHS App use only and not bound to a profile in the IG.<br>
		UKCoreSourceOfServiceRequest ValueSet are SNOMED CT Codes</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-PASEventType, text: PASEventType}}</td>
		<td>{{pagelink:CodeSystem-WPASEventType, text: WPASEventType}}</td>
		<td>For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-PASAdmitSource, text: PASAdmitSource}}</td>
		<td>{{pagelink:CodeSystem-WPASAdmitSource, text: WPASAdmitSource}}</td>
		<td>For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	</tbody>
</table>	

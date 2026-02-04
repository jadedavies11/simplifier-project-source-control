### {{page-title}}

The following Extensions are backported from R5 and are used in the implementation guide.


<style>
  th, td {
    word-wrap: break-word;
    white-space: normal;
  }
</style>

<table class="table table-striped" style="table-layout: fixed;">
  <colgroup>
    <col style="width: 14%;">
    <col style="width: 16%;">
    <col style="width: 24%;">
    <col style="width: 16%;">
    <col style="width: 16%;">
    <col style="width: 14%;">
  </colgroup>

  <thead>
    <tr>
      <th scope="col">Extension</th>
      <th scope="col">Bound to Profile</th>
      <th scope="col">Bound to Profile Element</th>
      <th scope="col">ValueSet</th>
      <th scope="col">CodeSystem</th>
      <th scope="col">DataType</th>
    </tr>
	</thead>
	<tbody>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-DocumentAttester}}</td>
			<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
			<td>extension:attesterR5</td>
			<td>
				<a href="https://hl7.org/fhir/valueset-composition-attestation-mode.html">composition-attestation-mode</a>
			</td>
			<td>
				<a href="https://hl7.org/fhir/codesystem-composition-attestation-mode.html">composition-attestation-mode</a>
			</td>
			<td>CodeableConcept, dateTime, Reference</td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-DocumentVersion}}</td>
			<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
			<td>extension:versionR5</td>
			<td></td>
			<td></td>
			<td>string</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483769">Extension-UKCore-DiagnosticReportComposition</a>
			</td>
			<td>{{pagelink:DataStandardsWales-DiagnosticReport}}</td>
			<td>extension:compositionReferenceR5</td>
			<td></td>
			<td></td>
			<td>Reference</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483769">Extension-UKCore-DiagnosticReportComposition</a>
			</td>
			<td>{{pagelink:DataStandardsWales-DiagnosticReport-Lab}}</td>
			<td>extension:compositionReferenceR5</td>
			<td></td>
			<td></td>
			<td>Reference</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483770">Extension-UKCore-DiagnosticReportNote</a>
			</td>
			<td>{{pagelink:DataStandardsWales-DiagnosticReport}}</td>
			<td>extension:noteR5</td>
			<td></td>
			<td></td>
			<td>Reference</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483770">Extension-UKCore-DiagnosticReportNote</a>
			</td>
			<td>{{pagelink:DataStandardsWales-DiagnosticReport-Lab}}</td>
			<td>extension:noteR5</td>
			<td></td>
			<td></td>
			<td>Reference</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483771">Extension-UKCore-DiagnosticReportSupportingInfo</a>
			</td>
			<td>{{pagelink:DataStandardsWales-DiagnosticReport}}</td>
			<td>extension:supportingInfoR5</td>
			<td>
				<a href="https://terminology.hl7.org/7.0.1/ValueSet-v2-0936.html">hl7VS-VS-observationType</a>
			</td>
			<td></td>
			<td>CodeableConcept, Reference</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483771">Extension-UKCore-DiagnosticReportSupportingInfo</a>
			</td>
			<td>{{pagelink:DataStandardsWales-DiagnosticReport-Lab}}</td>
			<td>extension:supportingInfoR5</td>
			<td>
				<a href="https://terminology.hl7.org/7.0.1/ValueSet-v2-0936.html">hl7VS-VS-observationType</a>
			</td>
			<td></td>
			<td>CodeableConcept, Reference</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483786">Extension-UKCore-ObservationBodyStructure</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation}}</td>
			<td>extension:bodyStructureR5</td>
			<td></td>
			<td></td>
			<td>Reference</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483786">Extension-UKCore-ObservationBodyStructure</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-Lab}}</td>
			<td>extension:bodyStructureR5</td>
			<td></td>
			<td></td>
			<td>Reference</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483786">Extension-UKCore-ObservationBodyStructure</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
			<td>extension:bodyStructureR5</td>
			<td></td>
			<td></td>
			<td>Reference</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483786">Extension-UKCore-ObservationBodyStructure</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
			<td>extension:bodyStructureR5</td>
			<td></td>
			<td></td>
			<td>Reference</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483786">Extension-UKCore-ObservationBodyStructure</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
			<td>extension:bodyStructureR5</td>
			<td></td>
			<td></td>
			<td>Reference</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483786">Extension-UKCore-ObservationBodyStructure</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
			<td>extension:bodyStructureR5</td>
			<td></td>
			<td></td>
			<td>Reference</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483787">Extension-UKCore-ObservationTriggeredBy</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation}}</td>
			<td>extension:triggeredByR5</td>
			<td>
				<a href="https://hl7.org/fhir/valueset-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>
				<a href="https://hl7.org/fhir/codesystem-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>Reference, code, string</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483787">Extension-UKCore-ObservationTriggeredBy</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-Lab}}</td>
			<td>extension:triggeredByR5</td>
			<td>
				<a href="https://hl7.org/fhir/valueset-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>
				<a href="https://hl7.org/fhir/codesystem-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>Reference, code, string</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483787">Extension-UKCore-ObservationTriggeredBy</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
			<td>extension:triggeredByR5</td>
			<td>
				<a href="https://hl7.org/fhir/valueset-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>
				<a href="https://hl7.org/fhir/codesystem-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>Reference, code, string</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483787">Extension-UKCore-ObservationTriggeredBy</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
			<td>extension:triggeredByR5</td>
			<td>
				<a href="https://hl7.org/fhir/valueset-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>
				<a href="https://hl7.org/fhir/codesystem-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>Reference, code, string</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483787">Extension-UKCore-ObservationTriggeredBy</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
			<td>extension:triggeredByR5</td>
			<td>
				<a href="https://hl7.org/fhir/valueset-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>
				<a href="https://hl7.org/fhir/codesystem-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>Reference, code, string</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483787">Extension-UKCore-ObservationTriggeredBy</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
			<td>extension:triggeredByR5</td>
			<td>
				<a href="https://hl7.org/fhir/valueset-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>
				<a href="https://hl7.org/fhir/codesystem-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>Reference, code, string</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483796">Extension-UKCore-SpecimenCollectionCollector</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Specimen}}</td>
			<td>collection.collector.extension:collectionCollectorR5</td>
			<td></td>
			<td></td>
			<td>Reference</td>
		</tr>
	</tbody>
</table>
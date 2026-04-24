### {{page-title}}

The following Extensions are backported from R5 and are used in the implementation guide.


<style>
  th, td {
    word-wrap: break-word;
    white-space: normal;
  }
     
    .small-text {
    font-size: 0.8rem;
  }
</style>

<table class="table table-striped" style="table-layout: fixed;">
  <colgroup>
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 24%;">
    <col style="width: 18%;">
    <col style="width: 18%;">
  </colgroup>

  <thead>
    <tr>
      <th scope="col">Extension</th>
      <th scope="col">Bound to Profile</th>
      <th scope="col">Bound to Profile Element</th>
      <th scope="col">ValueSet</th>
      <th scope="col">CodeSystem</th>
    </tr>
	</thead>
	<tbody>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-DocumentAttester, text:DataStandardsWales-DocumentAttester}}</td>
			<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
			<td class="small-text">DocumentReference.extension:attesterR5</td>
			<td>
				<a href="https://hl7.org/fhir/valueset-composition-attestation-mode.html">composition-attestation-mode</a>
			</td>
			<td>
				<a href="https://hl7.org/fhir/codesystem-composition-attestation-mode.html">composition-attestation-mode</a>
			</td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-DocumentVersion, text:DataStandardsWales-DocumentVersion}}</td>
			<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
			<td class="small-text">DocumentReference.extension:versionR5</td>
			<td></td>
			<td></td>
		</tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-Immunization.basedOn, text:DataStandardsWales-Immunization.basedOn}}</td>
			<td>{{pagelink:DataStandardsWales-Immunization}}</td>
			<td class="small-text">Immunization.extension:immunizationBasedOnR5</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483769">UKCore-DiagnosticReportComposition</a>
			</td>
			<td>{{pagelink:DataStandardsWales-DiagnosticReport}}</td>
			<td class="small-text">DiagnosticReport.extension:compositionReferenceR5</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483769">UKCore-DiagnosticReportComposition</a>
			</td>
			<td>{{pagelink:DataStandardsWales-DiagnosticReport-Lab}}</td>
			<td class="small-text">DiagnosticReport.extension:compositionReferenceR5</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483770">UKCore-DiagnosticReportNote</a>
			</td>
			<td>{{pagelink:DataStandardsWales-DiagnosticReport}}</td>
			<td class="small-text">DiagnosticReport.extension:noteR5</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483770">UKCore-DiagnosticReportNote</a>
			</td>
			<td>{{pagelink:DataStandardsWales-DiagnosticReport-Lab}}</td>
			<td class="small-text">DiagnosticReport.extension:noteR5</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483771">UKCore-DiagnosticReportSupportingInfo</a>
			</td>
			<td>{{pagelink:DataStandardsWales-DiagnosticReport}}</td>
			<td class="small-text">DiagnosticReport.extension:supportingInfoR5</td>
			<td>
				<a href="https://terminology.hl7.org/7.0.1/ValueSet-v2-0936.html">hl7VS-VS-observationType</a>
			</td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483771">UKCore-DiagnosticReportSupportingInfo</a>
			</td>
			<td>{{pagelink:DataStandardsWales-DiagnosticReport-Lab}}</td>
			<td class="small-text">DiagnosticReport.extension:supportingInfoR5</td>
			<td>
				<a href="https://terminology.hl7.org/7.0.1/ValueSet-v2-0936.html">hl7VS-VS-observationType</a>
			</td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483786">UKCore-ObservationBodyStructure</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation}}</td>
			<td class="small-text">Observation.extension:bodyStructureR5</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483786">UKCore-ObservationBodyStructure</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-Lab}}</td>
			<td class="small-text">Observation.extension:bodyStructureR5</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483786">UKCore-ObservationBodyStructure</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
			<td class="small-text">Observation.extension:bodyStructureR5</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483786">UKCore-ObservationBodyStructure</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
			<td class="small-text">Observation.extension:bodyStructureR5</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483786">UKCore-ObservationBodyStructure</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
			<td class="small-text">Observation.extension:bodyStructureR5</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483786">UKCore-ObservationBodyStructure</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
			<td class="small-text">Observation.extension:bodyStructureR5</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483787">UKCore-ObservationTriggeredBy</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation}}</td>
			<td class="small-text">Observation.extension:triggeredByR5</td>
			<td>
				<a href="https://hl7.org/fhir/valueset-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>
				<a href="https://hl7.org/fhir/codesystem-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483787">UKCore-ObservationTriggeredBy</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-Lab}}</td>
			<td class="small-text">Observation.extension:triggeredByR5</td>
			<td>
				<a href="https://hl7.org/fhir/valueset-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>
				<a href="https://hl7.org/fhir/codesystem-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483787">UKCore-ObservationTriggeredBy</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
			<td class="small-text">Observation.extension:triggeredByR5</td>
			<td>
				<a href="https://hl7.org/fhir/valueset-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>
				<a href="https://hl7.org/fhir/codesystem-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483787">UKCore-ObservationTriggeredBy</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
			<td class="small-text">Observation.extension:triggeredByR5</td>
			<td>
				<a href="https://hl7.org/fhir/valueset-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>
				<a href="https://hl7.org/fhir/codesystem-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483787">UKCore-ObservationTriggeredBy</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
			<td class="small-text">Observation.extension:triggeredByR5</td>
			<td>
				<a href="https://hl7.org/fhir/valueset-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>
				<a href="https://hl7.org/fhir/codesystem-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483787">UKCore-ObservationTriggeredBy</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
			<td class="small-text">Observation.extension:triggeredByR5</td>
			<td>
				<a href="https://hl7.org/fhir/valueset-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
			<td>
				<a href="https://hl7.org/fhir/codesystem-observation-triggeredbytype.html">observation-triggeredbytype</a>
			</td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483796">UKCore-SpecimenCollectionCollector</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Specimen}}</td>
			<td class="small-text">Specimen.collection.collector.extension:collectionCollectorR5</td>
			<td></td>
			<td></td>
		</tr>
	</tbody>
</table>
### {{page-title}}

The following UKCore ValueSets contain Welsh CodeSystems.

<style>
  th, td {
    word-wrap: break-word;
    white-space: normal;
  }
</style>

<table class="table table-striped" style="table-layout: fixed;">
  <colgroup>
    <col style="width: 18%;">
    <col style="width: 18%;">
    <col style="width: 14%;">
    <col style="width: 10%;">
    <col style="width: 18%;">
    <col style="width: 22%;">
  </colgroup>

  <thead>
    <tr>
      <th scope="col">ValueSet</th>
      <th scope="col">CodeSystem</th>
      <th scope="col">NHS Wales Standard</th>
      <th scope="col">ValueSet binding</th>
      <th scope="col">Bound to Profile</th>
      <th scope="col">Bound to element</th>
    </tr>
	</thead>
	<tbody>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483832">UKCore-AdmissionMethod</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483834">UKCore-AdmissionMethodWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483833">UKCore-AdmissionMethodEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/admissionmethod.htm">Admission Method</a>
		</td>
		<td>Extensible</td>
		<td>{{pagelink:DataStandardsWales-Encounter}}</td>
		<td>Encounter.hospitalization.extension:admissionMethod</td>
	</tr>
		<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483832">UKCore-AdmissionMethod</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483834">UKCore-AdmissionMethodWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483833">UKCore-AdmissionMethodEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/admissionmethod.htm">Admission Method</a>
		</td>
		<td>Extensible</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.hospitalization.extension:admissionMethod</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483856">UKCore-DischargeDestination</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483858">UKCore-DischargeDestinationWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483857">UKCore-DischargeDestinationEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/dischargedestination.htm">Discharge Destination</a>
		</td>
		<td>Preferred</td>
		<td>{{pagelink:DataStandardsWales-Encounter}}</td>
		<td>Encounter.hospitalization.dischargeDisposition</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483859">UKCore-DischargeMethod</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483861">UKCore-DischargeMethodWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483860">UKCore-DischargeMethodEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/dischargemethod.htm">Discharge Method</a>
		</td>
		<td>Extensible</td>
		<td>{{pagelink:DataStandardsWales-Encounter}}</td>
		<td>Encounter.extension:dischargeMethod</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483859">UKCore-DischargeMethod</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483861">UKCore-DischargeMethodWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483860">UKCore-DischargeMethodEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/dischargemethod.htm">Discharge Method</a>
		</td>
		<td>Extensible</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.extension:dischargeMethod</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483863">UKCore-EmergencyCareDischargeStatus</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483864">UKCore-EmergencyCareOutcomeOfAttendanceWales</a>
			&nbsp;SNOMED CT
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/outcomeofattendance.htm">Outcome of Attendance</a>
		</td>
		<td>Preferred</td>
		<td>{{pagelink:DataStandardsWales-Encounter}}</td>
		<td>Encounter.extension:emergencyCareDischargeStatus</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483863">UKCore-EmergencyCareDischargeStatus</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483864">UKCore-EmergencyCareOutcomeOfAttendanceWales</a>
			&nbsp;SNOMED CT
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/outcomeofattendance.htm">Outcome of Attendance</a>
		</td>
		<td>Preferred</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.extension:emergencyCareDischargeStatus</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483865">UKCore-EncounterLocationType</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483867">UKCore-EncounterLocationTypeWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483866">UKCore-EncounterLocationTypeEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/locationtypecode.htm">Location Type Code</a>
		</td>
		<td>Preferred</td>
		<td>{{pagelink:DataStandardsWales-Encounter}}</td>
		<td>Encounter.location.physicalType</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483865">UKCore-EncounterLocationType</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483867">UKCore-EncounterLocationTypeWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483866">UKCore-EncounterLocationTypeEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/locationtypecode.htm">Location Type Code</a>
		</td>
		<td>Preferred</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.location.physicalType</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483869">UKCore-EthnicCategory</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483871">UKCore-EthnicCategoryWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483870">UKCore-EthnicCategoryEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td>Extensible</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.extension:ethnicCategory</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483878">UKCore-LegalStatusClassification</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483880">UKCore-LegalStatusClassificationWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483879">UKCore-LegalStatusClassificationEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/legalstatus.htm">Legal Status</a>
		</td>
		<td>Extensible</td>
		<td>{{pagelink:DataStandardsWales-Encounter}}</td>
		<td>Encounter.extension:legalStatus</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483878">UKCore-LegalStatusClassification</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483880">UKCore-LegalStatusClassificationWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483879">UKCore-LegalStatusClassificationEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/legalstatus.htm">Legal Status</a>
		</td>
		<td>Extensible</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.extension:legalStatus</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483906">UKCore-NHSNumberVerificationStatus</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483908">UKCore-NHSNumberVerificationStatusWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483907">UKCore-LegalStatusClassificationEngland</a>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999019">v3.NullFlavor</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/nhsnumberstatusindicator.htm">NHS Number Status Indicator</a>
		</td>
		<td>Required</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.identifier:nhsNumber.extension:nhsNumberVerificationStatus</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483914">UKCore-OutcomeOfAttendance</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483916">UKCore-OutcomeOfAttendanceWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483915">UKCore-OutcomeOfAttendanceEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/outcomeofattendance.htm">Outcome of Attendance</a>
		</td>
		<td>Extensible</td>
		<td>{{pagelink:DataStandardsWales-Encounter}}</td>
		<td>Encounter.extension:OutcomeOfAttendance</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483914">UKCore-OutcomeOfAttendance</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483916">UKCore-OutcomeOfAttendanceWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483915">UKCore-OutcomeOfAttendanceEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/outcomeofattendance.htm">Outcome of Attendance</a>
		</td>
		<td>Extensible</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.extension:OutcomeOfAttendance</td>
	</tr>
		<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483919">UKCore-PersonMaritalStatusCode</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483921">UKCore-PersonMaritalStatusWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483920">UKCore-PersonMaritalStatusEngland</a>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2997937">v3.MaritalStatus</a>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999019">v3.NullFlavor</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td>Extensible</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.maritalStatus</td>
	</tr>
	</tr>
		<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483939">UKCore-SourceOfAdmission</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483941">UKCore-SourceOfAdmissionWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483940">UKCore-SourceOfAdmissionEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/sourceofadmission.htm">Source of Admission</a>
		</td>
		<td>Preferred</td>
		<td>{{pagelink:DataStandardsWales-Encounter}}</td>
		<td>Encounter.hospitalization.admitSource</td>
	</tr>
	</tbody>
</table>
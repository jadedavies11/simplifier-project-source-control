## {{page-title}}

The following Extensions contain Welsh data.

<style>
  th, td {
    word-wrap: break-word;
    white-space: normal;
  }
</style>

<table class="table table-striped" style="table-layout: fixed;">
  <colgroup>
    <col style="width: 18%;">
    <col style="width: 16%;">
    <col style="width: 16%;">
    <col style="width: 10%;">
    <col style="width: 18%;">
    <col style="width: 22%;">
  </colgroup>

  <thead>
    <tr>
      <th scope="col">Extension</th>
      <th scope="col">ValueSet</th>
      <th scope="col">CodeSystem</th>
      <th scope="col">NHS Wales Standard</th>
      <th scope="col">Bound to Profile</th>
      <th scope="col">Bound to element</th>
    </tr>
	</thead>
	<tbody>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
		</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-BodyPosition, text:DataStandardsWales-BodyPosition}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td>Observation.extension:bodyPosition</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
		</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-BodyPosition, text:DataStandardsWales-BodyPosition}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td>Observation.extension:bodyPosition</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
		</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-BodyPosition, text:DataStandardsWales-BodyPosition}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td>Observation.extension:bodyPosition</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
		</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-BodyPosition, text:DataStandardsWales-BodyPosition}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td>Observation.extension:bodyPosition</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-DocumentAttribute, text:DataStandardsWales-DocumentAttribute}}</td>
		<td>{{pagelink:ValueSet-FHIRStandardsWales-DocumentAttribute, text:FHIRStandardsWales-DocumentAttribute}}</td>
		<td>{{pagelink:CodeSystem-FHIRStandardsWales-DocumentAttribute, text:FHIRStandardsWales-DocumentAttribute}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>DocumentReference.extension:documentAttribute</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-DocumentDigitalStatus, text:DataStandardsWales-DocumentDigitalStatus}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-DocumentDigitalStatus, text:DataStandardsWales-DocumentDigitalStatus}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-DocumentDigitalStatus, text:DataStandardsWales-DocumentDigitalStatus}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>DocumentReference.extension:digitalStatus</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-DocumentErrorAction, text:DataStandardsWales-DocumentErrorAction}}</td>
		<td>{{pagelink:ValueSet-FHIRStandardsWales-DocumentErrorAction, text:FHIRStandardsWales-DocumentErrorAction}}</td>
		<td>{{pagelink:CodeSystem-FHIRStandardsWales-DocumentErrorAction, text:FHIRStandardsWales-DocumentErrorAction}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>DocumentReference.extension:errorAction</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-DocumentErrorStatus, text:DataStandardsWales-DocumentErrorStatus}}</td>
		<td>{{pagelink:ValueSet-FHIRStandardsWales-DocumentErrorStatus, text:FHIRStandardsWales-DocumentErrorStatus}}</td>
		<td>{{pagelink:CodeSystem-FHIRStandardsWales-DocumentErrorStatus, text:FHIRStandardsWales-DocumentErrorStatus}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>DocumentReference.extension:errorStatus</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-Occupation, text:DataStandardsWales-Occupation}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-Occupation, text:DataStandardsWales-Occupation}}</td>
		<td>SNOMED CT</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.extension:occupation</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td>VitalSigns Observation.extension:recordingSetting</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td>VitalSigns Observation.extension:recordingSetting</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td>VitalSigns Observation.extension:recordingSetting</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td>VitalSigns Observation.extension:recordingSetting</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-Religion, text:DataStandardsWales-Religion}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-Religion, text:DataStandardsWales-Religion}}</td>
		<td>SNOMED CT</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.extension:religion</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-UECAttendanceCategory, text:DataStandardsWales-UECAttendanceCategory}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-UEC-AttendanceCategory, text:DataStandardsWales-UEC-AttendanceCategory}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-UEC-AttendanceCategory, text:DataStandardsWales-UEC-AttendanceCategory}}</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.extension:uecAttendanceCategory</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2998643">modeOfArrival</a>
		</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-UEC-ArrivalMode, text:DataStandardsWales-UEC-ArrivalMode}}</td>
		<td>SNOMED CT</td>
		<td>
			<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.extension:modeOfArrival</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483753">UKCore-AdmissionMethod</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483832">UKCore-AdmissionMethod</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483834">UKCore-AdmissionMethodWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483833">UKCore-AdmissionMethodEngland</a>
		</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Encounter}}</td>
		<td>Encounter.hospitalization.extension:admissionMethod</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483753">UKCore-AdmissionMethod</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483832">UKCore-AdmissionMethod</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483834">UKCore-AdmissionMethodWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483833">UKCore-AdmissionMethodEngland</a>
		</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.hospitalization.extension:admissionMethod</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483772">UKCore-DischargeMethod</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483859">UKCore-DischargeMethod</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483861">UKCore-DischargeMethodWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483860">UKCore-DischargeMethodEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/dischargemethod.htm">Discharge Method</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter}}</td>
		<td>Encounter.extension:dischargeMethod</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483772">UKCore-DischargeMethod</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483859">UKCore-DischargeMethod</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483861">UKCore-DischargeMethodWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483860">UKCore-DischargeMethodEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/dischargemethod.htm">Discharge Method</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.extension:dischargeMethod</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483773">UKCore-EmergencyCareDischargeStatus</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483863">UKCore-EmergencyCareDischargeStatus</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483864">UKCore-EmergencyCareOutcomeOfAttendanceWales</a>
			&nbsp;SNOMED CT
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/outcomeofattendance.htm">Outcome of Attendance</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter}}</td>
		<td>Encounter.extension:emergencyCareDischargeStatus</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483773">UKCore-EmergencyCareDischargeStatus</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483863">UKCore-EmergencyCareDischargeStatus</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483864">UKCore-EmergencyCareOutcomeOfAttendanceWales</a>
			&nbsp;SNOMED CT
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/outcomeofattendance.htm">Outcome of Attendance</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.extension:emergencyCareDischargeStatus</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483774">UKCore-EthnicCategory</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483869">UKCore-EthnicCategory</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483871">UKCore-EthnicCategoryWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483870">UKCore-EthnicCategoryEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.extension:ethnicCategory</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483777">UKCore-LegalStatus</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483878">UKCore-LegalStatusClassification</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483880">UKCore-LegalStatusClassificationWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483879">UKCore-LegalStatusClassificationEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/legalstatus.htm">Legal Status</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter}}</td>
		<td>Encounter.extension:legalStatus</td>
	</tr>
		<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483777">UKCore-LegalStatus</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483878">UKCore-LegalStatusClassification</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483880">UKCore-LegalStatusClassificationWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483879">UKCore-LegalStatusClassificationEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/legalstatus.htm">Legal Status</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.extension:legalStatus</td>
	</tr>
	</tr>
		<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483785">UKCore-NHSNumberVerificationStatus</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483906">UKCore-NHSNumberVerificationStatus</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483908">UKCore-NHSNumberVerificationStatusWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483907">UKCore-NHSNumberVerificationStatusEngland</a>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999019">v3.NullFlavor</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/nhsnumberstatusindicator.htm">NHS Number Status Indicator</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.identifier:nhsNumber.extension:nhsNumberVerificationStatus</td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483789">UKCore-OutcomeOfAttendance</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483914">UKCore-OutcomeOfAttendance</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483916">UKCore-OutcomeOfAttendanceWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483915">UKCore-OutcomeOfAttendanceEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/outcomeofattendance.htm">Outcome of Attendance</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter}}</td>
		<td>Encounter.extension:OutcomeOfAttendance</td>
	</tr>
		<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483789">UKCore-OutcomeOfAttendance</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483914">UKCore-OutcomeOfAttendance</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483916">UKCore-OutcomeOfAttendanceWales</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483915">UKCore-OutcomeOfAttendanceEngland</a>
		</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/outcomeofattendance.htm">Outcome of Attendance</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.extension:OutcomeOfAttendance</td>
	</tr>
	</tbody>
</table>
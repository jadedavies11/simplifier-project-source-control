### {{page-title}}

The following Extensions have been defined for this implementation guide.


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
    <col style="width: 14%;">
    <col style="width: 18%;">
    <col style="width: 23%;">
    <col style="width: 18%;">
    <col style="width: 16%;">
    <col style="width: 11%;">
  </colgroup>

  <thead>
    <tr>
      <th scope="col">Extension</th>
      <th scope="col">Bound to Profile</th>
      <th scope="col">Bound to Profile Element</th>
      <th scope="col">ValueSet</th>
      <th scope="col">CodeSystem</th>
      <th scope="col">Backported</th>
    </tr>
	</thead>
	<tbody>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td class="small-text">Observation.extension:bodyPosition</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-BodyPosition, text:DataStandardsWalesBodyPosition}}</td>
		<td class="small-text">SNOMED CT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td class="small-text">Observation.extension:bodyPosition</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-BodyPosition, text:DataStandardsWalesBodyPosition}}
		</td>
		<td class="small-text">SNOMED CT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td class="small-text">Observation.extension:bodyPosition</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-BodyPosition, text:DataStandardsWalesBodyPosition}}
		</td>
		<td class="small-text">SNOMED CT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td class="small-text">Observation.extension:bodyPosition</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-BodyPosition, text:DataStandardsWalesBodyPosition}}
		</td>
		<td class="small-text">SNOMED CT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-AdministeredProduct, text: DataStandardsWales-AdministeredProduct}}</td>
		<td>{{pagelink:DataStandardsWales-Immunization}}</td>
		<td class="small-text">Immunization.extension:administeredProduct</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-ClinicCode, text: DataStandardsWales-ClinicCode}}</td>
		<td>{{pagelink:DataStandardsWales-Appointment}}</td>
		<td class="small-text">Appointment.extension:clinicCode</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-DateProcedureLastUpdated, text: DataStandardsWales-DateProcedureLastUpdated}}</td>
		<td>{{pagelink:DataStandardsWales-Immunization}}</td>
		<td class="small-text">Immunization.extension:dateProcedureLastUpdated</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-DemographicsAsRecorded, text: DataStandardsWales-DemographicsAsRecorded}}</td>
		<td>{{pagelink:DataStandardsWales-Provenance}}</td>
		<td class="small-text">Provenance.extension:extensionDataStandardsWalesDemographicsAsRecorded</td>
		<td>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/3001742">AdministrativeGender</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/3001376">AdministrativeGender</a>
		</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-DocumentAttester, text: DataStandardsWales-DocumentAttester}}</td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td class="small-text">DocumentReference.extension:attesterR5</td>
		<td>
			<a href="https://hl7.org/fhir/valueset-composition-attestation-mode.html">composition-attestation-mode</a>
		</td>
		<td>
			<a href="https://hl7.org/fhir/codesystem-composition-attestation-mode.html">composition-attestation-mode</a>
		</td>
		<td>R5</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-DocumentAttribute, text: DataStandardsWales-DocumentAttribute}}</td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td class="small-text">DocumentReference.extension:documentAttribute</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-DocumentAttribute, text:DataStandardsWales-DocumentAttribute}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-DocumentAttribute, text:DataStandardsWales-DocumentAttribute}}</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-DocumentDigitalStatus, text: DataStandardsWales-DocumentDigitalStatus}}</td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td class="small-text">DocumentReference.extension:digitalStatus</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-DocumentDigitalStatus, text:DataStandardsWales-DocumentDigitalStatus}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-DocumentDigitalStatus, text:DataStandardsWales-DocumentDigitalStatus}}</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-DocumentErrorAction, text: DataStandardsWales-DocumentErrorAction}}</td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td class="small-text">DocumentReference.extension:errorAction</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-DocumentErrorAction, text:DataStandardsWales-DocumentErrorAction}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-DocumentErrorAction, text:DataStandardsWales-DocumentErrorAction}}</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-DocumentErrorStatus, text: DataStandardsWales-DocumentErrorStatus}}</td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td class="small-text">DocumentReference.extension:errorStatus</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-DocumentErrorStatus, text:DataStandardsWales-DocumentErrorStatus}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-DocumentErrorStatus, text:DataStandardsWales-DocumentErrorStatus}}</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-DocumentVersion, text: DataStandardsWales-DocumentVersion}}</td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td class="small-text">DocumentReference.extension:versionR5</td>
		<td></td>
		<td></td>
		<td>R5</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-ForecastCreationSource, text: DataStandardsWales-ForecastCreationSource}}</td>
		<td>{{pagelink:DataStandardsWales-Immunization}}</td>
		<td class="small-text">Immunization.extension:forecastCreationSource</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-Immunization.basedOn, text: DataStandardsWales-Immunization.basedOn}}</td>
		<td>{{pagelink:DataStandardsWales-Immunization}}</td>
		<td class="small-text">Immunization.extension:immunizationBasedOnR5</td>
		<td></td>
		<td></td>
		<td>R5</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-MedicationCourseOfTherapyType, text: DataStandardsWales-MedicationCourseOfTherapyType}}</td>
		<td>{{pagelink:DataStandardsWales-MedicationStatement}}</td>
		<td class="small-text">MedicationStatement.extension:medicationCourseOfTherapyType</td>
		<td>
			<a href="https://terminology.hl7.org/7.0.1/ValueSet-medicationrequest-course-of-therapy.html">Medication request course of therapy codes</a>
		</td>
		<td>
			<a href="https://terminology.hl7.org/7.0.1/CodeSystem-medicationrequest-course-of-therapy.html">MedicationRequest Course of Therapy Codes</a>
		</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-Occupation, text: DataStandardsWales-Occupation}}</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td class="small-text">Patient.extension:occupation</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-Occupation}}</td>
		<td class="small-text">SNOMED CT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td class="small-text">Observation.extension:recordingSetting</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td class="small-text">Observation.extension:recordingSetting</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td class="small-text">Observation.extension:recordingSetting</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td class="small-text">Observation.extension:recordingSetting</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-Religion, text: DataStandardsWales-Religion}}</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td class="small-text">Patient.extension:religion</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-Religion, text:DataStandardsWales-Religion}}</td>
		<td class="small-text">SNOMED CT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-SingleRecord-AllergiesListConfirmedBy, text:DataStandardsWales-SingleRecord-AllergiesListConfirmedBy}}</td>
		<td>{{pagelink:DataStandardsWales-AllergyList}}</td>
		<td class="small-text">List.extension:SingleRecordAllergiesListConfirmedBy</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-SingleRecord-AllergiesListConfirmedDate, text: DataStandardsWales-SingleRecord-AllergiesListConfirmedDate}}</td>
		<td>{{pagelink:DataStandardsWales-AllergyList}}</td>
		<td class="small-text">List.extension:SingleRecordAllergiesListConfirmedDate</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-SingleRecord-AllergiesListUpdated, text: DataStandardsWales-SingleRecord-AllergiesListUpdated}}</td>
		<td>{{pagelink:DataStandardsWales-AllergyList}}</td>
		<td class="small-text">List.extension:SingleRecordAllergiesListUpdated</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-SourceSystem, text: DataStandardsWales-SourceSystem}}</td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td class="small-text">DocumentReference.extension:sourceSystem</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-Speciality, text: DataStandardsWales-Speciality}}</td>
		<td>{{pagelink:DataStandardsWales-Encounter}}</td>
		<td class="small-text">Encounter.extension:Speciality</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483924">UKCore-PracticeSettingCode</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483923">UKCore-PracticeSettingCode</a>
		</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-Speciality, text: DataStandardsWales-Speciality}}</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td class="small-text">Encounter.extension:Speciality</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483924">UKCore-PracticeSettingCode</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483923">UKCore-PracticeSettingCode</a>
		</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-UECAttendanceCategory, text: DataStandardsWales-UECAttendanceCategory}}</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td class="small-text">Encounter.extension:uecAttendanceCategory</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-UEC-AttendanceCategory, text:DataStandardsWales-UEC-AttendanceCategory}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-UEC-AttendanceCategory, text:DataStandardsWales-UEC-AttendanceCategory}}</td>	
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-UECDischargeInformationGiven, text: DataStandardsWales-UECDischargeInformationGiven}}</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td class="small-text">Encounter.extension:uecDischargeInformationGiven</td>
		<td></td>
		<td></td>	
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink: Extension-DataStandardsWales-UECExpectedTimeOfTreatment, text: DataStandardsWales-UECExpectedTimeOfTreatment}}</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td class="small-text">Encounter.extension:uecExpectedTimeOfTreatment</td>
		<td></td>
		<td></td>	
		<td></td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2998643">modeOfArrival</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td class="small-text">Encounter.extension:modeOfArrival</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-UEC-ArrivalMode, text:DataStandardsWales-UEC-ArrivalMode}}</td>
		<td class="small-text">SNOMED CT</td>
		<td></td>
	</tr>	
	</tbody>
</table>


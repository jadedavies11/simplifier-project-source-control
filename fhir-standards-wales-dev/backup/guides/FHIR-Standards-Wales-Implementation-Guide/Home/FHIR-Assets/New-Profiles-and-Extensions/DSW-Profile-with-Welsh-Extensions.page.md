### {{page-title}}

This is a list of Data Standards Wales profiles with extensions to be used in NHS Wales.


<style>
  th, td {
    word-wrap: break-word;
    white-space: normal;
  }
</style>

<table class="table table-striped" style="table-layout: fixed;">
  <colgroup>
    <col style="width: 12%;">
    <col style="width: 16%;">
    <col style="width: 21%;">
    <col style="width: 18%;">
    <col style="width: 12%;">
    <col style="width: 12%;">
    <col style="width: 9%;">
  </colgroup>

  <thead>
    <tr>
      <th scope="col">Profile</th>
      <th scope="col">Extension</th>
      <th scope="col">Bound to Profile Element</th>
      <th scope="col">ValueSet & CodeSystem</th>
      <th scope="col">DataType</th>
      <th scope="col">NHS Wales Standard</th>
      <th scope="col">Backported</th>
    </tr>
	</thead>
	<tbody>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-AllergyList}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-SingleRecord-AllergiesListConfirmedBy, text:DataStandardsWales-SingleRecord-AllergiesListConfirmedBy}}</td>
		<td>extension:SingleRecordAllergiesListConfirmedBy</td>
		<td></td>
		<td>Reference</td>
		<td></td>
		<td></td>
	</tr>	
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-AllergyList}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-SingleRecord-AllergiesListConfirmedDate, text:DataStandardsWales-SingleRecord-AllergiesListConfirmedDate}}</td>
		<td>extension:SingleRecordAllergiesListConfirmedDate</td>
		<td></td>
		<td>dateTime</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-AllergyList}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-SingleRecord-AllergiesListUpdated, text:DataStandardsWales-SingleRecord-AllergiesListUpdated}}</td>
		<td>extension:SingleRecordAllergiesListUpdated</td>
		<td></td>
		<td>boolean</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Appointment}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-ClinicCode, text:DataStandardsWales-ClinicCode}}</td>
		<td>extension:clinicCode</td>
		<td></td>
		<td>string</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-DocumentAttester, text:DataStandardsWales-DocumentAttester}}</td>
		<td>extension:attesterR5</td>
		<td>
			<a href="https://hl7.org/fhir/valueset-composition-attestation-mode.html">composition-attestation-mode</a>
			<a href="https://hl7.org/fhir/codesystem-composition-attestation-mode.html">composition-attestation-mode</a>
		</td>
		<td>CodeableConcept, dateTime, Reference</td>
		<td></td>
		<td>R5</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-DocumentAttribute, text:DataStandardsWales-DocumentAttribute}}</td>
		<td>extension:documentAttribute</td>
		<td> 
			<a href="https://simplifier.net/fhir-standards-wales/fhirstandardswales-documentattribute">FHIRStandardsWales-DocumentAttribute</a>
			<a href="https://simplifier.net/fhir-standards-wales/fhirstandardswales-documentattribute-duplicate-2">FHIRStandardsWales-DocumentAttribute</a>
		</td>
		<td>code, string</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-DocumentDigitalStatus, text:DataStandardsWales-DocumentDigitalStatus}}</td>
		<td>extension:digitalStatus</td>
		<td>
			<a href="https://simplifier.net/fhir-standards-wales/datastandardswales-documentdigitalstatus">DataStandardsWales-DocumentDigitalStatus</a>
			<a href="https://simplifier.net/fhir-standards-wales/datastandardswales-documentdigitalstatus-duplicate-2">DataStandardsWales-DocumentDigitalStatus</a>
		</td>
		<td>code</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-DocumentErrorAction, text:DataStandardsWales-DocumentErrorAction}}</td>
		<td>extension:errorAction</td>
		<td></td>
		<td>code, instant, Reference, CodeableConcept</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-DocumentErrorStatus, text:DataStandardsWales-DocumentErrorStatus}}</td>
		<td>extension:errorStatus</td>
		<td></td>
		<td>code</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-DocumentVersion, text:DataStandardsWales-DocumentVersion}}</td>
		<td>extension:versionR5</td>
		<td></td>
		<td>string</td>
		<td></td>
		<td>R5</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-SourceSystem, text:DataStandardsWales-SourceSystem}}</td>
		<td>extension:sourceSystem</td>
		<td></td>
		<td>Reference</td>
		<td></td>
		<td></td>
	</tr>
		<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Encounter}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-Speciality, text:DataStandardsWales-Speciality}}</td>
		<td>extension:Speciality</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483924">UKCore-PracticeSettingCode</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483923">UKCore-PracticeSettingCode</a>
		</td>
		<td>CodeableConcept</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-Speciality, text:DataStandardsWales-Speciality}}</td>
		<td>extension:Speciality</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483924">UKCore-PracticeSettingCode</a>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483923">UKCore-PracticeSettingCode</a>
		</td>
		<td>CodeableConcept</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-UECAttendanceCategory, text:DataStandardsWales-UEC-AttendanceCategory}}</td>
		<td>Encounter.extension:uecAttendanceCategory</td>
		<td>
			<a href="https://simplifier.net/fhir-standards-wales/datastandardswales-uec-attendancecategory">DataStandardsWales-UEC-AttendanceCategory</a>
			<a href="https://simplifier.net/fhir-standards-wales/datastandardswales-uec-attendancecategory-duplicate-2">DataStandardsWales-UEC-AttendanceCategory</a>
		</td>
		<td>CodeableConcept</td>	
		<td>
			<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
		</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-UECDischargeInformationGiven, text:DataStandardsWales-UEC-DischargeInformationGiven}}</td>
		<td>extension:uecDischargeInformationGiven</td>
		<td></td>
		<td>boolean, Reference</td>	
		<td>
			<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
		</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-UECExpectedTimeOfTreatment, text:DataStandardsWales-UEC-ExpectedTimeOfTreatment}}</td>
		<td>extension:uecExpectedTimeOfTreatment</td>
		<td></td>
		<td>dateTime</td>	
		<td>
			<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
		</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Encounter-UEC}}</td>	
		<td>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2998643">modeOfArrival</a>
		</td>
		<td>extension:modeOfArrival</td>
		<td>
			<a href="https://simplifier.net/fhir-standards-wales/datastandardswales-uec-arrivalmode">DataStandardsWales-UEC-ArrivalMode</a>
			&nbsp;SNOMED CT	
		</td>
		<td>Coding</td>
		<td>
			<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
		</td>		
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Immunization}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-AdministeredProduct, text:DataStandardsWales-AdministeredProduct}}</td>
		<td>extension:DataStandardsWalesAdministeredProduct</td>
		<td></td>
		<td>Reference</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Immunization}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-DateProcedureLastUpdated, text:DataStandardsWales-DateProcedureLastUpdated}}</td>
		<td>extension:DataStandardsWalesDateProcedureLastUpdated</td>
		<td></td>
		<td>dateTime</td>
		<td></td>
		<td></td>
	</tr>	
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Immunization}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-ForecastCreationSource, text:DataStandardsWales-ForecastCreationSource}}</td>
		<td>extension:DataStandardsWalesForecastCreationSource</td>
		<td></td>
		<td>Annotation</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Immunization}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-Immunization.basedOn, text:DataStandardsWales-Immunization.basedOn}}</td>
		<td>extension:DataStandardsWalesImmunizationBasedOn</td>
		<td></td>
		<td>Reference</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-MedicationStatement}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-MedicationCourseOfTherapyType, text:DataStandardsWales-MedicationCourseOfTherapyType}}</td>
		<td>extension:medicationCourseOfTherapyType</td>
		<td>
			<a href="https://terminology.hl7.org/7.0.1/ValueSet-medicationrequest-course-of-therapy.html">Medication request course of therapy codes</a>
			<a href="https://terminology.hl7.org/7.0.1/CodeSystem-medicationrequest-course-of-therapy.html">MedicationRequest Course of Therapy Codes</a>
		</td>
		<td>CodeableConcept</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>extension:recordingSetting</td>
		<td>
			<a href="https://simplifier.net/fhir-standards-wales/datastandardswales-recordingsetting-duplicate-2">DataStandardsWales-RecordingSetting</a>
			<a href="https://simplifier.net/fhir-standards-wales/datastandardswales-recordingsetting">DataStandardsWales-RecordingSetting</a>
		</td>
		<td>CodeableConcept</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td>	
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
		</td>
		<td>extension:bodyPosition</td>
		<td>
			<a href="https://fhir.nhs.wales/ValueSet/DataStandardsWales-BodyPosition">DataStandardsWalesBodyPosition</a>
			&nbsp;SNOMED CT
		</td>
		<td>CodeableConcept</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>extension:recordingSetting</td>
		<td>
			<a href="https://simplifier.net/fhir-standards-wales/datastandardswales-recordingsetting-duplicate-2">DataStandardsWales-RecordingSetting</a>
			<a href="https://simplifier.net/fhir-standards-wales/datastandardswales-recordingsetting">DataStandardsWales-RecordingSetting</a>
		</td>
		<td>CodeableConcept</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td>	
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
		</td>
		<td>extension:bodyPosition</td>
		<td>
			<a href="https://fhir.nhs.wales/ValueSet/DataStandardsWales-BodyPosition">DataStandardsWalesBodyPosition</a>
			&nbsp;SNOMED CT
		</td>
		<td>CodeableConcept</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>extension:recordingSetting</td>
		<td>
			<a href="https://simplifier.net/fhir-standards-wales/datastandardswales-recordingsetting-duplicate-2">DataStandardsWales-RecordingSetting</a>
			<a href="https://simplifier.net/fhir-standards-wales/datastandardswales-recordingsetting">DataStandardsWales-RecordingSetting</a>
		</td>
		<td>CodeableConcept</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td>	
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
		</td>
		<td>extension:bodyPosition</td>
		<td>
			<a href="https://fhir.nhs.wales/ValueSet/DataStandardsWales-BodyPosition">DataStandardsWalesBodyPosition</a>
			&nbsp;SNOMED CT
		</td>
		<td>CodeableConcept</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-RecordingSetting, text:DataStandardsWales-RecordingSetting}}</td>
		<td>extension:recordingSetting</td>
		<td>
			<a href="https://simplifier.net/fhir-standards-wales/datastandardswales-recordingsetting-duplicate-2">DataStandardsWales-RecordingSetting</a>
			<a href="https://simplifier.net/fhir-standards-wales/datastandardswales-recordingsetting">DataStandardsWales-RecordingSetting</a>
		</td>
		<td>CodeableConcept</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td>	
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
		</td>
		<td>extension:bodyPosition</td>
		<td>
			<a href="https://fhir.nhs.wales/ValueSet/DataStandardsWales-BodyPosition">DataStandardsWalesBodyPosition</a>
			&nbsp;SNOMED CT
		</td>
		<td>CodeableConcept</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Patient}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-Occupation, text:DataStandardsWales-Occupation}}</td>
		<td>extension:occupation</td>
		<td>
			<a href="https://simplifier.net/fhir-standards-wales/datastandardswales-occupation">DataStandardsWales-Occupation</a>
			&nbsp;SNOMED CT
		</td>
		<td>CodeableConcept</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Patient}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-Religion, text:DataStandardsWales-Religion}}</td>
		<td>Patient.extension:religion</td>
		<td>
			<a href="https://simplifier.net/fhir-standards-wales/datastandardswales-religion">DataStandardsWales-Religion</a>
			&nbsp;SNOMED CT
		</td>
		<td>CodeableConcept</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Provenance}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-DemographicsAsRecorded, text:DataStandardsWales-DemographicsAsRecorded}}</td>
		<td>extension:extensionDataStandardsWalesDemographicsAsRecorded</td>
		<td>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/3001742">AdministrativeGender</a>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/3001376">AdministrativeGender</a>
		</td>
		<td>Address, code, HumanName, dateTime, Identifier</td>
		<td></td>
		<td></td>
	</tbody>
</table>
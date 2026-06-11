
This is a list of Data Standards Wales profiles with local extensions to be used in NHS Wales.


<style>
  th, td {
    word-wrap: break-word;
    white-space: normal;
  }
</style>

<table class="table table-striped" style="table-layout: fixed;">
  <colgroup>
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
	<col style="width: 20%;">
  </colgroup>

  <thead>
    <tr>
      <th scope="col">Profile</th>
      <th scope="col">Extension</th>
      <th scope="col">Bound to Profile Element</th>
      <th scope="col">ValueSet</th>
	  <th scope="col">CodeSystem</th>
    </tr>
	</thead>
	<tbody>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-AllergyList}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-SingleRecord-AllergiesListConfirmedBy, text:DataStandardsWales-SingleRecord-AllergiesListConfirmedBy}}</td>
		<td>extension:SingleRecordAllergiesListConfirmedBy</td>
		<td></td>
		<td></td>
	</tr>	
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-AllergyList}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-SingleRecord-AllergiesListConfirmedDate, text:DataStandardsWales-SingleRecord-AllergiesListConfirmedDate}}</td>
		<td>extension:SingleRecordAllergiesListConfirmedDate</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-AllergyList}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-SingleRecord-AllergiesListUpdated, text:DataStandardsWales-SingleRecord-AllergiesListUpdated}}</td>
		<td>extension:SingleRecordAllergiesListUpdated</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Appointment}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-ClinicCode, text:DataStandardsWales-ClinicCode}}</td>
		<td>extension:clinicCode</td>
		<td></td>
		<td></td>
	<tr>
    </tr>
    <tr>
		<td scope="row">{{pagelink:DataStandardsWales-Encounter}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-Speciality, text:DataStandardsWales-Speciality}}</td>
		<td>extension:Speciality</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483924">UKCore-PracticeSettingCode</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483923">UKCore-PracticeSettingCode</a>
		</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-Speciality, text:DataStandardsWales-Speciality}}</td>
		<td>extension:Speciality</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483924">UKCore-PracticeSettingCode</a>	
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483923">UKCore-PracticeSettingCode</a>
		</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-UECAttendanceCategory, text:DataStandardsWales-UEC-AttendanceCategory}}</td>
		<td>Encounter.extension:uecAttendanceCategory</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-UEC-AttendanceCategory, text:DataStandardsWales-UEC-AttendanceCategory}}
		</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-UEC-AttendanceCategory, text:DataStandardsWales-UEC-AttendanceCategory}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-UECDischargeInformationGiven, text:DataStandardsWales-UEC-DischargeInformationGiven}}</td>
		<td>extension:uecDischargeInformationGiven</td>
		<td></td>
		<td></td>	
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-UECExpectedTimeOfTreatment, text:DataStandardsWales-UEC-ExpectedTimeOfTreatment}}</td>
		<td>extension:uecExpectedTimeOfTreatment</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Encounter-UEC}}</td>	
		<td>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2998643">modeOfArrival</a>
		</td>
		<td>extension:modeOfArrival</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-UEC-ArrivalMode, text:DataStandardsWales-UEC-ArrivalMode}}</td>
		<td>SNOMED CT</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Immunization}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-AdministeredProduct, text:DataStandardsWales-AdministeredProduct}}</td>
		<td>extension:administeredProduct</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Immunization}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-DateProcedureLastUpdated, text:DataStandardsWales-DateProcedureLastUpdated}}</td>
		<td>extension:dateProcedureLastUpdated</td>
		<td></td>
		<td></td>
	</tr>	
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Immunization}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-ForecastCreationSource, text:DataStandardsWales-ForecastCreationSource}}</td>
		<td>extension:forecastCreationSource</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-MedicationStatement}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-MedicationCourseOfTherapyType, text:DataStandardsWales-MedicationCourseOfTherapyType}}</td>
		<td>extension:medicationCourseOfTherapyType</td>
		<td>
			<a href="https://terminology.hl7.org/7.0.1/ValueSet-medicationrequest-course-of-therapy.html">Medication request course of therapy codes</a>	
		</td>
		<td>
			<a href="https://terminology.hl7.org/7.0.1/CodeSystem-medicationrequest-course-of-therapy.html">MedicationRequest Course of Therapy Codes</a>
		</td>
	</tr>
    <tr>
		<td scope="row">{{pagelink:DataStandardsWales-Organization}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-AliasType, text:DataStandardsWales-AliasType}}</td>
		<td>extension:aliasType</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-AliasType, text:DataStandardsWales-AliasType}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-AliasType, text:DataStandardsWales-AliasType}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Patient}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-Occupation, text:DataStandardsWales-Occupation}}</td>
		<td>extension:occupation</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-Occupation, text:DataStandardsWales-Occupation}}</td>
		<td>SNOMED CT</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Patient}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-Religion, text:DataStandardsWales-Religion}}</td>
		<td>Patient.extension:religion</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-Religion, text:DataStandardsWales-Religion}}</td>
		<td>SNOMED CT</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:DataStandardsWales-Provenance}}</td>
		<td>{{pagelink:Extension-DataStandardsWales-DemographicsAsRecorded, text:DataStandardsWales-DemographicsAsRecorded}}</td>
		<td>extension:extensionDataStandardsWalesDemographicsAsRecorded</td>
		<td>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/3001742">AdministrativeGender</a><br>
		</td>
		<td>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/3001376">AdministrativeGender</a>
		</td>
    </tr>
	</tbody>
</table>
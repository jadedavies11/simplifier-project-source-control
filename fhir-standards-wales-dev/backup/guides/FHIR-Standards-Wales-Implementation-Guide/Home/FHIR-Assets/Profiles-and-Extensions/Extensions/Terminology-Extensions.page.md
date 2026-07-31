The Extensions created for this Implementation Guide are listed with the Profiles they extend and associated terminologies where relevant.


<style>
  th, td {
    word-wrap: break-word;
    white-space: normal;
  }
    
</style>

<table class="table table-striped" style="table-layout: fixed;">
  <colgroup>
    <col style="width: 16%;">
    <col style="width: 20%;">
    <col style="width: 24%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
  </colgroup>

  <thead>
    <tr>
      <th scope="col">Extension</th>
      <th scope="col">Profile Extended</th>
      <th scope="col">Profile Element Extended</th>
      <th scope="col">ValueSet</th>
      <th scope="col">CodeSystem</th>
    </tr>
	</thead>
	<tbody>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-AdministeredProduct}}</td>
		<td>{{pagelink:DataStandardsWales-Immunization}}</td>
		<td style="font-size: 90%;">Immunization.extension:administeredProduct</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
		<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-AliasType}}</td>
		<td>{{pagelink:DataStandardsWales-Organization}}</td>
		<td style="font-size: 90%;">Organization.alias.extension:aliasType</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-AliasType}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-AliasType}}</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-ClinicCode}}</td>
		<td>{{pagelink:DataStandardsWales-Appointment}}</td>
		<td style="font-size: 90%;">Appointment.extension:clinicCode</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-DateProcedureLastUpdated}}</td>
		<td>{{pagelink:DataStandardsWales-Immunization}}</td>
		<td style="font-size: 90%;">Immunization.extension:dateProcedureLastUpdated</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-DemographicsAsRecorded}}</td>
		<td>{{pagelink:DataStandardsWales-Provenance}}</td>
		<td style="font-size: 90%;">Provenance.extension:extensionDataStandardsWalesDemographicsAsRecorded</td>
		<td>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/3001742">AdministrativeGender</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/3001376">AdministrativeGender</a>
		</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-DocumentDigitalStatus}}</td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td style="font-size: 90%;">DocumentReference.extension:digitalStatus</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-DocumentDigitalStatus}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-DocumentDigitalStatus}}</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-ForecastCreationSource}}</td>
		<td>{{pagelink:DataStandardsWales-Immunization}}</td>
		<td style="font-size: 90%;">Immunization.extension:forecastCreationSource</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-MedicationCourseOfTherapyType}}</td>
		<td>{{pagelink:DataStandardsWales-MedicationStatement}}</td>
		<td style="font-size: 90%;">MedicationStatement.extension:medicationCourseOfTherapyType</td>
		<td>
			<a href="https://terminology.hl7.org/7.0.1/ValueSet-medicationrequest-course-of-therapy.html">Medication request course of therapy codes</a>
		</td>
		<td>
			<a href="https://terminology.hl7.org/7.0.1/CodeSystem-medicationrequest-course-of-therapy.html">MedicationRequest Course of Therapy Codes</a>
		</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-Occupation}}</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td style="font-size: 90%;">Patient.extension:occupation</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-Occupation}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-Religion}}</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td style="font-size: 90%;">Patient.extension:religion</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-Religion}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-SingleRecord-AllergiesListConfirmedBy}}</td>
		<td>{{pagelink:DataStandardsWales-AllergyList}}</td>
		<td style="font-size: 90%;">List.extension:SingleRecordAllergiesListConfirmedBy</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-SingleRecord-AllergiesListConfirmedDate}}</td>
		<td>{{pagelink:DataStandardsWales-AllergyList}}</td>
		<td style="font-size: 90%;">List.extension:SingleRecordAllergiesListConfirmedDate</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-SingleRecord-AllergiesListUpdated}}</td>
		<td>{{pagelink:DataStandardsWales-AllergyList}}</td>
		<td style="font-size: 90%;">List.extension:SingleRecordAllergiesListUpdated</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-Speciality}}</td>
		<td>{{pagelink:DataStandardsWales-Encounter}}</td>
		<td style="font-size: 90%;">Encounter.extension:Speciality</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483924">ValueSet-UKCore-PracticeSettingCode</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483923">CodeSystem-UKCore-PracticeSettingCode</a>
		</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-Speciality}}</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td style="font-size: 90%;">Encounter.extension:Speciality</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483924">ValueSet-UKCore-PracticeSettingCode</a>
		</td>
		<td>
			<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483923">CodeSystem-UKCore-PracticeSettingCode</a>
		</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-UECAttendanceCategory}}</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td style="font-size: 90%;">Encounter.extension:uecAttendanceCategory</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-UEC-AttendanceCategory}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-UEC-AttendanceCategory}}</td>	
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-UECDischargeInformationGiven}}</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td style="font-size: 90%;">Encounter.extension:uecDischargeInformationGiven</td>
		<td></td>
		<td></td>	
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:Extension-DataStandardsWales-UECExpectedTimeOfTreatment}}</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td style="font-size: 90%;">Encounter.extension:uecExpectedTimeOfTreatment</td>
		<td></td>
		<td></td>	
		<td></td>
	</tr>
	<tr>
		<td scope="row">
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2998643">modeOfArrival</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td style="font-size: 90%;">Encounter.extension:modeOfArrival</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-UEC-ArrivalMode}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td></td>
	</tr>	
	</tbody>
</table>
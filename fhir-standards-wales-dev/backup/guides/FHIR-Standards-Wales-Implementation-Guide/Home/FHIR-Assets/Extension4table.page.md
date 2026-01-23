### {{page-title}}

The following Extensions have been defined for this implementation guide.


<table class="table table-striped">
	<thead>
		<tr>
			<th scope="col">Extension</th>
			<th scope="col">Bound to Profile</th>
			<th scope="col">Bound to Profile Element</th>
			<th scope="col">ValueSet</th>
			<th scope="col">CodeSystem</th>
			<th scope="col">NHS Wales Standard</th>
			<th scope="col">Backported</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
			<td>Observation.extension:bodyPosition</td>
			<td>
				<a href="https://fhir.nhs.wales/ValueSet/DataStandardsWales-BodyPosition">DataStandardsWalesBodyPosition</a>
			</td>
			<td>SNOMED CT/td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
			<td>Observation.extension:bodyPosition</td>
			<td>
				<a href="https://fhir.nhs.wales/ValueSet/DataStandardsWales-BodyPosition">DataStandardsWalesBodyPosition</a>
			</td>
			<td>SNOMED CT/td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
			<td>Observation.extension:bodyPosition</td>
			<td>
				<a href="https://fhir.nhs.wales/ValueSet/DataStandardsWales-BodyPosition">DataStandardsWalesBodyPosition</a>
			</td>
			<td>SNOMED CT/td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999538">bodyPosition</a>
			</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
			<td>Observation.extension:bodyPosition</td>
			<td>
				<a href="https://fhir.nhs.wales/ValueSet/DataStandardsWales-BodyPosition">DataStandardsWalesBodyPosition</a>
			</td>
			<td>SNOMED CT/td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-AdministeredProduct}}</td>
			<td>{{pagelink:DataStandardsWales-Immunization}}</td>
			<td>Immunization.extension:DataStandardsWalesAdministeredProduct</td>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-ClinicCode}}</td>
			<td>{{pagelink:DataStandardsWales-Appointment}}</td>
			<td>Appointment.extension:clinicCode</td>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-DateProcedureLastUpdated}}</td>
			<td>{{pagelink:DataStandardsWales-Immunization}}</td>
			<td>Immunization.extension:DataStandardsWalesDateProcedureLastUpdated</td>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-DemographicsAsRecorded}}</td>
			<td>{{pagelink:DataStandardsWales-Provenance}}</td>
			<td>Provenance.extension:extensionDataStandardsWalesDemographicsAsRecorded</td>
			<td>
				<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/3001742">AdministrativeGender</a>
			</td>
			<td>
				<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/3001376">AdministrativeGender</a>
			</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-DocumentAttester}}</td>
			<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
			<td>DocumentReference.extension:attesterR5</td>
			<td>
				<a href="https://hl7.org/fhir/valueset-composition-attestation-mode.html">composition-attestation-mode</a>
			</td>
			<td>
				<a href="https://hl7.org/fhir/codesystem-composition-attestation-mode.html">composition-attestation-mode</a>
			</td>
			<td></td>
			<td>R5 Backport</td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-DocumentAttribute}}</td>
			<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
			<td>DocumentReference.extension:documentAttribute</td>
			<td>{{pagelink:ValueSet-FHIRStandardsWales-DocumentAttribute}}</td>
			<td>{{pagelink:CodeSystem-FHIRStandardsWales-DocumentAttribute}}</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-DocumentDigitalStatus}}</td>
			<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
			<td>DocumentReference.extension:digitalStatus</td>
			<td>{{pagelink:ValueSet-DataStandardsWales-DocumentDigitalStatus}}</td>
			<td>{{pagelink:CodeSystem-DataStandardsWales-DocumentDigitalStatus}}</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-DocumentErrorAction}}</td>
			<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
			<td>DocumentReference.extension:errorAction</td>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-DocumentErrorStatus}}</td>
			<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
			<td>DocumentReference.extension:errorStatus</td>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-DocumentVersion}}</td>
			<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
			<td>DocumentReference.extension:versionR5</td>
			<td></td>
			<td></td>
			<td></td>
			<td>R5 Backport</td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-ForecastCreationSource}}</td>
			<td>{{pagelink:DataStandardsWales-Immunization}}</td>
			<td>Immunization.extension:DataStandardsWalesForecastCreationSource</td>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-Immunization.basedOn}}</td>
			<td>{{pagelink:DataStandardsWales-Immunization}}</td>
			<td>Immunization.extension:DataStandardsWalesImmunizationBasedOn</td>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-MedicationCourseOfTherapyType}}</td>
			<td>{{pagelink:DataStandardsWales-MedicationStatement}}</td>
			<td>MedicationStatement.extension:medicationCourseOfTherapyType</td>
			<td>
				<a href="https://terminology.hl7.org/7.0.1/ValueSet-medicationrequest-course-of-therapy.html">Medication request course of therapy codes</a>
			</td>
			<td>
				<a href="https://terminology.hl7.org/7.0.1/CodeSystem-medicationrequest-course-of-therapy.html">MedicationRequest Course of Therapy Codes</a>
			</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-Occupation}}</td>
			<td>{{pagelink:DataStandardsWales-Patient}}</td>
			<td>Patient.extension:occupation</td>
			<td>{{pagelink:ValueSet-DataStandardsWales-Occupation}}</td>
			<td>SNOMED CT</td>
			<td>
				<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
			</td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-RecordingSetting}}</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
			<td>Observation.extension:recordingSetting</td>
			<td>{{pagelink: ValueSet-DataStandardsWales-RecordingSetting}}</td>
			<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting}}</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-RecordingSetting}}</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
			<td>Observation.extension:recordingSetting</td>
			<td>{{pagelink: ValueSet-DataStandardsWales-RecordingSetting}}</td>
			<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting}}</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-RecordingSetting}}</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
			<td>Observation.extension:recordingSetting</td>
			<td>{{pagelink: ValueSet-DataStandardsWales-RecordingSetting}}</td>
			<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting}}</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-RecordingSetting}}</td>
			<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
			<td>Observation.extension:recordingSetting</td>
			<td>{{pagelink: ValueSet-DataStandardsWales-RecordingSetting}}</td>
			<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting}}</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-Religion}}</td>
			<td>{{pagelink:DataStandardsWales-Patient}}</td>
			<td>Patient.extension:religion</td>
			<td>{{pagelink:ValueSet-DataStandardsWales-Religion}}</td>
			<td>SNOMED CT</td>
			<td>
				<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
			</td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-SingleRecord-AllergiesListConfirmedBy}}</td>
			<td>{{pagelink:DataStandardsWales-AllergyList}}</td>
			<td>List.extension:SingleRecordAllergiesListConfirmedBy</td>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-SingleRecord-AllergiesListConfirmedDate}}</td>
			<td>{{pagelink:DataStandardsWales-AllergyList}}</td>
			<td>List.extension:SingleRecordAllergiesListConfirmedDate</td>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-SingleRecord-AllergiesListUpdated}}</td>
			<td>{{pagelink:DataStandardsWales-AllergyList}}</td>
			<td>List.extension:SingleRecordAllergiesListUpdated</td>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-SourceSystem}}</td>
			<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
			<td>DocumentReference.extension:sourceSystem</td>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-Speciality}}</td>
			<td>{{pagelink:DataStandardsWales-Encounter}}</td>
			<td>Encounter.extension:Speciality</td>
			<td>
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483924">ValueSet-UKCore-PracticeSettingCode</a>
			</td>
			<td>
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483923">CodeSystem-UKCore-PracticeSettingCode</a>
			</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-Speciality}}</td>
			<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
			<td>Encounter.extension:Speciality</td>
			<td>
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483924">ValueSet-UKCore-PracticeSettingCode</a>
			</td>
			<td>
				<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483923">CodeSystem-UKCore-PracticeSettingCode</a>
			</td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-UECAttendanceCategory}}</td>
			<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
			<td>Encounter.extension:uecAttendanceCategory</td>
			<td>{{pagelink:ValueSet-DataStandardsWales-UEC-AttendanceCategory}}</td>
			<td>{{pagelink:CodeSystem-DataStandardsWales-UEC-AttendanceCategory}}</td>	
			<td>
				<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
			</td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-UECDischargeInformationGiven}}</td>
			<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
			<td>Encounter.extension:uecDischargeInformationGiven</td>
			<td></td>
			<td></td>	
			<td>
				<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
			</td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">{{pagelink:Extension-DataStandardsWales-UECExpectedTimeOfTreatment}}</td>
			<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
			<td>Encounter.extension:uecExpectedTimeOfTreatment</td>
			<td></td>
			<td></td>	
			<td>
				<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
			</td>
			<td></td>
		</tr>
		<tr>
			<td scope="row">
				<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2998643">modeOfArrival/a>
			</td>
			<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
			<td>Encounter.extension:modeOfArrival</td>
			<td>{{pagelink:ValueSet-DataStandardsWales-UEC-ArrivalMode}}</td>
			<td>SNOMED CT</td>	
			<td>
				<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
			</td>
			<td></td>
		</tr>
	</tbody>
</table>


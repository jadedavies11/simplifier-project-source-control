The following ValueSets have been defined for this Implementation Guide.

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
      <th scope="col">ValueSet</th>
      <th scope="col">CodeSystem</th>
      <th scope="col">Bound to Profile</th>
      <th scope="col">Bound to element</th>
      <th scope="col">Additional information</th>
    </tr>
	</thead>
	<tbody>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BloodPressure-AverageSystolic}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td></td>
		<td></td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BloodPressure-Diastolic}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td></td>
		<td></td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BMI}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td style="font-size: 90%;">Observation.code.coding:snomedCT</td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BodyHeightMeasurements}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td style="font-size: 90%;">Observation.code.coding:snomedCT</td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BodyPosition}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td style="font-size: 90%;">Observation.extension:bodyPosition</td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BodyPosition}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td style="font-size: 90%;">Observation.extension:bodyPosition</td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BodyPosition}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td style="font-size: 90%;">Observation.extension:bodyPosition</td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BodyPosition}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td style="font-size: 90%;">Observation.extension:bodyPosition</td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BodyTemperature}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td></td>
		<td></td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
	</tr>
		<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BodyWeightMeasurements}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td style="font-size: 90%;">Observation.code.coding:snomedCT</td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
	</tr>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-DocumentCategory}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td style="font-size: 90%;">DocumentReference.category</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-DocumentDigitalStatus}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-DocumentDigitalStatus}}</td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td style="font-size: 90%;">DocumentReference.extension:digitalStatus</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-DocumentType}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td style="font-size: 90%;">DocumentReference.type</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-EncounterType}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-UEC-CareConsultationMechanism}}<br>
		{{pagelink:CodeSystem-DataStandardsWales-UEC-ActivityType}}<br>&<br>
		&nbsp;<span style="font-size: 80%;">SNOMED CT</span>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td style="font-size: 90%;">Encounter.type</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-GenderIdentity}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-GenderIdentity}}</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td style="font-size: 90%;">Patient.gender</td>
		<td style="font-size: 90%;">Used for mapping</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-HeadCircumferenceMeasurements}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td></td>
		<td></td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-HeartRate}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td></td>
		<td></td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-MainSpecialty}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-MainSpecialty}}</td>
		<td></td>
		<td></td>
		<td style="font-size: 90%;">Not bound to profile</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-MaritalStatus}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-MaritalStatus}}</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td style="font-size: 90%;">Patient.maritalStatus</td>
		<td style="font-size: 90%;">Used for mapping</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-MessageEvent}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-UEC-MessageEvent}}<br>
		{{pagelink:CodeSystem-MessageEvents}}
		</td>
		<td>{{pagelink:DataStandardsWales-MessageDefinition}}</td>
		<td style="font-size: 90%;">MessageDefinition.event</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td style="font-size: 90%;">Observation.code.coding:snomedCT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td style="font-size: 90%;">Observation.component.code</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td style="font-size: 90%;">Observation.component.code.coding:snomedCT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td style="font-size: 90%;">Observation.component.code</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td style="font-size: 90%;">Observation.component.code.coding:snomedCT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td style="font-size: 90%;">Observation.component.code</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td style="font-size: 90%;">Observation.component.code.coding:snomedCT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td style="font-size: 90%;">Observation.component.code</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td style="font-size: 90%;">Observation.component.code.coding:snomedCT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-Occupation}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td style="font-size: 90%;">Patient.extension:occupation</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-OxygenSaturation}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td></td>
		<td></td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-PatientRecordType}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Provenance}}</td>
		<td></td>
		<td style="font-size: 90%;">For CDR use only and not bound to a profile in the IG</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ProvenanceActivity}}</td>
		<td>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999499">ISO 21089-2017 Health Record Lifecycle Events</a>
		</td>
		<td></td>
		<td style="font-size: 90%;">Provenance.activity</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td style="font-size: 90%;">Observation.extension:recordingSetting</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td style="font-size: 90%;">Observation.extension:recordingSetting</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td style="font-size: 90%;">Observation.extension:recordingSetting</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td style="font-size: 90%;">Observation.extension:recordingSetting</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-RespirationRate}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td></td>
		<td></td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-Religion}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td style="font-size: 90%;">Patient.extension:religion</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-Sex}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-Sex}}</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td style="font-size: 90%;">Patient.extension:birthSex</td>
		<td style="font-size: 90%;">Used for mapping</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-Title}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-Title}}</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td style="font-size: 90%;">Patient.name.prefix</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-UEC-Acuity}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td style="font-size: 90%;">Encounter.priority</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-UEC-ArrivalMode}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td style="font-size: 90%;">Encounter.extension:modeOfArrival</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-UEC-AttendanceCategory}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-UEC-AttendanceCategory}}</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td style="font-size: 90%;">Encounter.extension:uecAttendanceCategory</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-UEC-AttendanceSource}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td style="font-size: 90%;">Encounter.hospitalization.admitSource</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-UEC-DischargeDestination}}</td>
		<td style="font-size: 80%;">SNOMED CT</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td style="font-size: 90%;">Encounter.hospitalization.dischargeDisposition</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-MessageEvents}}</td>
		<td>{{pagelink:CodeSystem-MessageEvents}}</td>
		<td>{{pagelink:DataStandardsWales-MessageDefinition}}</td>
		<td style="font-size: 90%;">MessageDefinition.event</td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-MessageEvent}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-MessageEvents}}</td>
		<td>{{pagelink:CodeSystem-MessageEvents}}</td>
		<td>{{pagelink:DataStandardsWales-MessageHeader}}</td>
		<td style="font-size: 90%;">MessageHeader.event</td>
		<td style="font-size: 90%;">Embedded in<br>{{pagelink:ValueSet-DataStandardsWales-MessageEvent}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-PASAdmitSource}}</td>
		<td>{{pagelink:CodeSystem-WPASAdmitSource}}</td>
		<td></td>
		<td></td>
		<td style="font-size: 90%;">For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-PASEventType}}</td>
		<td>{{pagelink:CodeSystem-WPASEventType}}</td>
		<td></td>
		<td></td>
		<td style="font-size: 90%;">For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-PASReferralSource}}</td>
		<td>{{pagelink:CodeSystem-WPASReferralSource}}<br>&<br>
		&nbsp;<span style="font-size: 80%;">SNOMED CT</span>
		</td>
		<td></td>
		<td></td>
		<td style="font-size: 90%;">For CDR/ NHS App use only and not bound to a profile in the IG.<br>The SCT codes are
<a href="https://simplifier.net/packages/fhir.r4.ukcore.stu2/2.0.1/files/2483937">UKCoreSourceOfServiceRequest</a> ValueSet</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-PASSourceAdmission}}</td>
		<td>{{pagelink:CodeSystem-WPASSourceAdmission}}</td>
		<td></td>
		<td></td>
		<td style="font-size: 90%;">For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	</tbody>
</table>
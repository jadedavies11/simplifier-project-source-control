### {{page-title}}

The following ValueSets have been defined for this implementation guide.

<style>
  th, td {
    word-wrap: break-word;
    white-space: normal;
  }
</style>

<table class="table table-striped" style="table-layout: fixed;">
  <colgroup>
    <col style="width: 16%;">
    <col style="width: 16%;">
    <col style="width: 16%;">
    <col style="width: 16%;">
    <col style="width: 16%;">
    <col style="width: 20%;">
  </colgroup>

  <thead>
    <tr>
      <th scope="col">ValueSet</th>
      <th scope="col">CodeSystem</th>
      <th scope="col">NHS Wales Standard</th>
      <th scope="col">Bound to Profile</th>
      <th scope="col">Bound to element</th>
      <th scope="col">Additional information</th>
    </tr>
	</thead>
	<tbody>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BloodPressure-AverageSystolic, text: DataStandardsWales-BloodPressure-AverageSystolic}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td></td>
		<td></td>
		<td>Embedded in {{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWalesObservationVitalSignsType}} ValueSet</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BloodPressure-Diastolic, text: DataStandardsWales-BloodPressure-Diastolic}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td></td>
		<td></td>
		<td>Embedded in {{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWalesObservationVitalSignsType}} ValueSet</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BMI, text: DataStandardsWales-BMI}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td>Observation.code.coding:snomedCT</td>
		<td>Embedded in {{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWalesObservationVitalSignsType}} ValueSet too</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BodyHeightMeasurements, text: DataStandardsWales-BodyHeightMeasurements}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td>Observation.code.coding:snomedCT</td>
		<td>Embedded in {{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWalesObservationVitalSignsType}} ValueSet too</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BodyPosition, text: DataStandardsWales-BodyPosition}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td>Observation.extension:bodyPosition</td>
		<td>Embedded in {{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWalesObservationVitalSignsType}} ValueSet too</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BodyPosition, text: DataStandardsWales-BodyPosition}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td>Observation.extension:bodyPosition</td>
		<td>Embedded in {{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWalesObservationVitalSignsType}} ValueSet too</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BodyPosition, text: DataStandardsWales-BodyPosition}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td>Observation.extension:bodyPosition</td>
		<td>Embedded in {{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWalesObservationVitalSignsType}} ValueSet too</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BodyPosition, text: DataStandardsWales-BodyPosition}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td>Observation.extension:bodyPosition</td>
		<td>Embedded in {{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWalesObservationVitalSignsType}} ValueSet too</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BodyTemperature, text: DataStandardsWales-BodyTemperature}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td></td>
		<td></td>
		<td>Embedded in {{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWalesObservationVitalSignsType}} ValueSet</td>
	</tr>
		<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-BodyWeightMeasurements, text: DataStandardsWales-BodyWeightMeasurements}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td>Observation.code.coding:snomedCT</td>
		<td>Embedded in {{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWalesObservationVitalSignsType}} ValueSet too</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-DocumentCategory, text: DataStandardsWales-DocumentCategory}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-DocumentCategory, text: DataStandardsWales-DocumentCategory}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>DocumentReference.category</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-DocumentDigitalStatus, text: DataStandardsWales-DocumentDigitalStatus}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-DocumentDigitalStatus, text: DataStandardsWales-DocumentDigitalStatus}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>DocumentReference.extension:digitalStatus</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-DocumentType, text: DataStandardsWales-DocumentType}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>DocumentReference.type</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-EncounterType, text: DataStandardsWales-EncounterType}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-UEC-CareConsultationMechanism, text: DataStandardsWales-UEC-CareConsultationMechanism}}<br>
		{{pagelink:CodeSystem-DataStandardsWales-UEC-ActivityType, text: DataStandardsWales-UEC-ActivityType}}<br>
			&nbsp;SNOMED CT	
		</td>
		<td>
			<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.type</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-GenderIdentity, text: DataStandardsWales-GenderIdentity}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-GenderIdentity, text: DataStandardsWales-GenderIdentity}}</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.gender</td>
		<td>Used for mapping</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-HeadCircumferenceMeasurements, text: DataStandardsWales-HeadCircumferenceMeasurements}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td></td>
		<td></td>
		<td>Embedded in {{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWalesObservationVitalSignsType}} ValueSet</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-HeartRate, text: DataStandardsWales-HeartRate}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td></td>
		<td></td>
		<td>Embedded in {{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWalesObservationVitalSignsType}} ValueSet</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-MainSpecialty, text: DataStandardsWales-MainSpecialty}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-MainSpecialty, text: DataStandardsWales-MainSpecialty}}</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/mainspecialtyconsultant.htm">Main Specialty (Consultant)</a>
		</td>
		<td></td>
		<td></td>
		<td>Not bound to profile</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-MaritalStatus, text: DataStandardsWales-MaritalStatus}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-MaritalStatus, text: DataStandardsWales-MaritalStatus}}</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.maritalStatus</td>
		<td>Used for mapping</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-MessageEvent, text: DataStandardsWales-MessageEvent}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-UEC-MessageEvent, text: DataStandardsWales-UEC-MessageEvent}}<br>
		{{pagelink:CodeSystem-MessageEvents, text: MessageEvents}}
		</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-MessageDefinition}}</td>
		<td>MessageDefinition.event</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWales-ObservationVitalSignsType}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td>Observation.code.coding:snomedCT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWales-ObservationVitalSignsType}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td>Observation.component.code</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWales-ObservationVitalSignsType}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td>Observation.component.code.coding:snomedCT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWales-ObservationVitalSignsType}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td>Observation.component.code</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWales-ObservationVitalSignsType}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td>Observation.component.code.coding:snomedCT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWales-ObservationVitalSignsType}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td>Observation.component.code</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWales-ObservationVitalSignsType}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td>Observation.component.code.coding:snomedCT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWales-ObservationVitalSignsType}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td>Observation.component.code</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWales-ObservationVitalSignsType}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td>Observation.component.code.coding:snomedCT</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-Occupation, text: DataStandardsWales-Occupation}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.extension:occupation</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-OxygenSaturation, text: DataStandardsWales-OxygenSaturation}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td></td>
		<td></td>
		<td>Embedded in {{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWalesObservationVitalSignsType}} ValueSet</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-ProvenanceActivity, text: DataStandardsWales-ProvenanceActivity}}</td>
		<td>
			<a href="https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/2999499">ISO 21089-2017 Health Record Lifecycle Events</a>
		</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Provenance}}</td>
		<td>Provenance.activity</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td>Observation.extension:recordingSetting</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td>Observation.extension:recordingSetting</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td>Observation.extension:recordingSetting</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td>Observation.extension:recordingSetting</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-RespirationRate, text: DataStandardsWales-RespirationRate}}</td>
		<td>SNOMED CT</td>
		<td></td>
		<td></td>
		<td></td>
		<td>Embedded in {{pagelink:ValueSet-DataStandardsWales-ObservationVitalSignsType, text: DataStandardsWalesObservationVitalSignsType}} ValueSet</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-Religion, text: DataStandardsWales-Religion}}</td>
		<td>SNOMED CT</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.extension:religion</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-Sex, text: DataStandardsWales-Sex}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-Sex, text: DataStandardsWales-Sex}}</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.extension:birthSex</td>
		<td>Used for mapping</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-Title, text: DataStandardsWales-Title}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-Title, text: DataStandardsWales-Title}}</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.name.prefix</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-UEC-Acuity, text: DataStandardsWales-UEC-Acuity}}</td>
		<td>SNOMED CT</td>
		<td>
			<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.priority</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-UEC-ArrivalMode, text: DataStandardsWales-UEC-ArrivalMode}}</td>
		<td>SNOMED CT</td>
		<td>
			<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.extension:modeOfArrival</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-UEC-AttendanceCategory, text: DataStandardsWales-UEC-AttendanceCategory}}</td>
		<td>{{pagelink:CodeSystem-DataStandardsWales-UEC-AttendanceCategory, text: DataStandardsWales-UEC-AttendanceCategory}}</td>
		<td>
			<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.extension:uecAttendanceCategory</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-UEC-AttendanceSource, text: DataStandardsWales-UEC-AttendanceSource}}</td>
		<td>SNOMED CT</td>
		<td>
			<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.hospitalization.admitSource</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-DataStandardsWales-UEC-DischargeDestination, text: DataStandardsWales-UEC-DischargeDestination}}</td>
		<td>SNOMED CT</td>
		<td>
			<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.hospitalization.dischargeDisposition</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-FHIRStandardsWales-DocumentAttribute, text: FHIRStandardsWales-DocumentAttribute}}</td>
		<td>{{pagelink:CodeSystem-FHIRStandardsWales-DocumentAttribute, text: FHIRStandardsWales-DocumentAttribute}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>DocumentReference.extension:documentAttribute</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-FHIRStandardsWales-DocumentErrorAction, text: FHIRStandardsWales-DocumentErrorAction}}</td>
		<td>{{pagelink:CodeSystem-FHIRStandardsWales-DocumentErrorAction, text: FHIRStandardsWales-DocumentErrorAction}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>DocumentReference.extension:errorAction</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-FHIRStandardsWales-DocumentErrorStatus, text: FHIRStandardsWales-DocumentErrorStatus}}</td>
		<td>{{pagelink:CodeSystem-FHIRStandardsWales-DocumentErrorStatus, text: FHIRStandardsWales-DocumentErrorStatus}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>DocumentReference.extension:errorStatus</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-MessageEvents, text: MessageEvents}}</td>
		<td>{{pagelink:CodeSystem-MessageEvents, text: MessageEvents}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-MessageDefinition}}</td>
		<td>MessageDefinition.event</td>
		<td>Embedded in DataStandardsWalesMessageEvent ValueSet</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-MessageEvents, text: MessageEvents}}</td>
		<td>{{pagelink:CodeSystem-MessageEvents, text: MessageEvents}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-MessageHeader}}</td>
		<td>MessageHeader.event</td>
		<td>Embedded in DataStandardsWalesMessageEvent ValueSet</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-PASAdmitSource, text: PASAdmitSource}}</td>
		<td>{{pagelink:CodeSystem-WPASAdmitSource, text: WPASAdmitSource}}</td>
		<td></td>
		<td></td>
		<td></td>
		<td>For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-PASEventType, text: PASEventType}}</td>
		<td>{{pagelink:CodeSystem-WPASEventType, text: WPASEventType}}</td>
		<td></td>
		<td></td>
		<td></td>
		<td>For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-PASReferralSource, text: PASReferralSource}}</td>
		<td>{{pagelink:CodeSystem-WPASReferralSource, text: WPASReferralSource}}&nbsp;SNOMED CT</td>
		<td></td>
		<td></td>
		<td></td>
		<td>For CDR/ NHS App use only and not bound to a profile in the IG.<br>The SCT codes are UKCoreSourceOfServiceRequest ValueSet</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:ValueSet-PASSourceAdmission, text: PASSourceAdmission}}</td>
		<td>{{pagelink:CodeSystem-WPASSourceAdmission, text: WPASSourceAdmission}}</td>
		<td></td>
		<td></td>
		<td></td>
		<td>For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	</tbody>
</table>
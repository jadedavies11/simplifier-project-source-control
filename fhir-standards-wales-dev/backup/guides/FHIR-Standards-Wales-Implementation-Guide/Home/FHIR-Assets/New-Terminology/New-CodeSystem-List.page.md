### {{page-title}}

The following CodeSystems have been defined for this implementation guide.

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
      <th scope="col">CodeSystem</th>
      <th scope="col">ValueSet</th>
      <th scope="col">NHS Wales Standard</th>
      <th scope="col">Bound to Profile</th>
      <th scope="col">Bound to element</th>
      <th scope="col">Additional information</th>
    </tr>
	</thead>
	<tbody>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-DocumentCategory, text: DataStandardsWales-DocumentCategory}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-DocumentCategory, text: DataStandardsWales-DocumentCategory}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>DocumentReference.category</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-DocumentDigitalStatus, text: DataStandardsWales-DocumentDigitalStatus}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-DocumentDigitalStatus, text: DataStandardsWales-DocumentDigitalStatus}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>DocumentReference.extension:digitalStatus</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-GenderIdentity, text: DataStandardsWales-GenderIdentity}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-GenderIdentity, text: DataStandardsWales-GenderIdentity}}</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.gender</td>
		<td>Used for mapping</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-MainSpecialty, text: DataStandardsWales-MainSpecialty}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-MainSpecialty, text: DataStandardsWales-MainSpecialty}}</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/mainspecialtyconsultant.htm">Main Specialty (Consultant)</a>
		</td>
		<td></td>
		<td></td>
		<td>Not bound to profile</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-MaritalStatus, text: DataStandardsWales-MaritalStatus}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-MaritalStatus, text: DataStandardsWales-MaritalStatus}}</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.maritalStatus</td>
		<td>Used for mapping</td>
	</tr>
		<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-PatientRecordType, text: DataStandardsWales-PatientRecordType}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-PatientRecordType, text: DataStandardsWales-PatientRecordType}}</td>
		<td></td>
		<td></td>
		<td></td>
		<td>Not bound to profile</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td>Observation.extension:recordingSetting</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td>Observation.extension:recordingSetting</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td>Observation.extension:recordingSetting</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting, text: DataStandardsWales-RecordingSetting}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td>Observation.extension:recordingSetting</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-Sex, text: DataStandardsWales-Sex}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-Sex, text: DataStandardsWales-Sex}}</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.extension:birthSex</td>
		<td>Used for mapping</td>
	</tr>
		<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-Title, text: DataStandardsWales-Title}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-Title, text: DataStandardsWales-Title}}</td>
		<td>
			<a href="https://www.datadictionary.wales.nhs.uk/#!WordDocuments/corereferencedatastandards1.htm">Core Reference Data Standards</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td>Patient.name.prefix</td>
		<td></td>
	</tr>
		<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-UEC-ActivityType, text: DataStandardsWales-UEC-ActivityType}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-EncounterType, text: DataStandardsWales-EncounterType}}</td>
		<td>
			<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.type</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-UEC-AttendanceCategory, text: DataStandardsWales-UEC-AttendanceCategory}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-UEC-AttendanceCategory, text: DataStandardsWales-UEC-AttendanceCategory}}</td>
		<td>
			<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.extension:uecAttendanceCategory</td>
		<td></td>
	</tr>
		<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-UEC-CareConsultationMechanism, text: DataStandardsWales-UEC-CareConsultationMechanism}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-EncounterType, text: DataStandardsWales-EncounterType}}</td>
		<td>
			<a href="https://dhcw.nhs.wales/data/information-standards/data-standards/data-standards-files/data-standard-change-notices-docs/dscns-2024/20240718-dscn-2024-12-welsh-emergency-care-data-set-0-3-2-pdf1/">Welsh Emergency Care Data 
Set</a>
		</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td>Encounter.type</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-UEC-MessageEvent, text: DataStandardsWales-UEC-MessageEvent}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-MessageEvent, text: DataStandardsWales-MessageEvent}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-MessageDefinition}}</td>
		<td>MessageDefinition.event</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-UEC-MessageEvent, text: DataStandardsWales-UEC-MessageHeader}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-MessageEvent, text: DataStandardsWales-MessageEvent}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-MessageDefinition}}</td>
		<td>MessageHeader.event</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-FHIRStandardsWales-DocumentAttribute, text: FHIRStandardsWales-DocumentAttribute}}</td>
		<td>{{pagelink:ValueSet-FHIRStandardsWales-DocumentAttribute, text: FHIRStandardsWales-DocumentAttribute}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>DocumentReference.extension:documentAttribute</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-FHIRStandardsWales-DocumentErrorAction, text: FHIRStandardsWales-DocumentErrorAction}}</td>
		<td>{{pagelink:ValueSet-FHIRStandardsWales-DocumentErrorAction, text: FHIRStandardsWales-DocumentErrorAction}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>DocumentReference.extension:errorAction</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-FHIRStandardsWales-DocumentErrorStatus, text: FHIRStandardsWales-DocumentErrorStatus}}</td>
		<td>{{pagelink:ValueSet-FHIRStandardsWales-DocumentErrorStatus, text: FHIRStandardsWales-DocumentErrorStatus}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td>DocumentReference.extension:errorStatus</td>
		<td></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-MessageEvents, text: MessageEvents}}</td>
		<td>{{pagelink:ValueSet-MessageEvents, text: MessageEvents}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-MessageDefinition}}</td>
		<td>MessageDefinition.event</td>
		<td>Embedded in DataStandardsWalesMessageEvent ValueSet</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-MessageEvents, text: MessageEvents}}</td>
		<td>{{pagelink:ValueSet-MessageEvents, text: MessageEvents}}</td>
		<td></td>
		<td>{{pagelink:DataStandardsWales-MessageHeader}}</td>
		<td>MessageHeader.event</td>
		<td>Embedded in DataStandardsWalesMessageEvent ValueSet</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-WPASAdmitSource, text: WPASAdmitSource}}</td>
		<td>{{pagelink:ValueSet-PASAdmitSource, text: PASAdmitSource}}</td>
		<td></td>
		<td></td>
		<td></td>
		<td>For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-WPASEventType, text: WPASEventType}}</td>
		<td>{{pagelink:ValueSet-PASEventType, text: PASEventType}}</td>
		<td></td>
		<td></td>
		<td></td>
		<td>For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-WPASReferralSource, text: WPASReferralSource}}</td>
		<td>{{pagelink:ValueSet-PASReferralSource, text: PASReferralSource}}</td>
		<td></td>
		<td></td>
		<td></td>
		<td>For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-WPASSourceAdmission, text: WPASSourceAdmission}}</td>
		<td>{{pagelink:ValueSet-PASSourceAdmission, text: PASSourceAdmission}}</td>
		<td></td>
		<td></td>
		<td></td>
		<td>For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	</tbody>
</table>
The following Code Systems have been defined for this Implementation Guide and are listed along with additional narrative

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
      <th scope="col">Code System</th>
      <th scope="col">Value Set</th>
      <th scope="col">Bound to Profile</th>
      <th scope="col">Bound to element</th>
      <th scope="col">Additional information</th>
    </tr>
	</thead>
	<tbody>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-AliasType}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-AliasType}}</td>
		<td>{{pagelink:DataStandardsWales-Location}}</td>
		<td style="font-size: 90%;">Location.alias.extension:aliasType</td>
		<td style="font-size: 90%;"></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-AliasType}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-AliasType}}</td>
		<td>{{pagelink:DataStandardsWales-Organization}}</td>
		<td style="font-size: 90%;">Organization.alias.extension:aliasType</td>
		<td style="font-size: 90%;"></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-DocumentDigitalStatus}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-DocumentDigitalStatus}}</td>
		<td>{{pagelink:DataStandardsWales-DocumentReference}}</td>
		<td style="font-size: 90%;">DocumentReference.extension:digitalStatus</td>
		<td style="font-size: 90%;"></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-GenderIdentity}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-GenderIdentity}}</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td style="font-size: 90%;">Patient.gender</td>
		<td style="font-size: 90%;">Used for mapping</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-LocationForm}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-LocationForm}}</td>
		<td>{{pagelink:DataStandardsWales-Location}}</td>
		<td style="font-size: 90%;">Location.physicalType</td>
		<td style="font-size: 90%;"></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-LocationType}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-LocationType}}</td>
		<td>{{pagelink:DataStandardsWales-Location}}</td>
		<td style="font-size: 90%;">Location.type:locationType</td>
		<td style="font-size: 90%;"></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-LocationTypeCategory}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-LocationTypeCategory}}</td>
		<td>{{pagelink:DataStandardsWales-Location}}</td>
		<td style="font-size: 90%;">Location.type:locationCategory</td>
		<td style="font-size: 90%;"></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-MainSpecialty}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-MainSpecialty}}</td>
		<td></td>
		<td style="font-size: 90%;"></td>
		<td style="font-size: 90%;">Not bound to profile</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-MaritalStatus}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-MaritalStatus}}</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td style="font-size: 90%;">Patient.maritalStatus</td>
		<td style="font-size: 90%;">Used for mapping</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-MessageEvent}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-MessageEvent}}</td>
		<td>{{pagelink:DataStandardsWales-MessageDefinition}}</td>
		<td style="font-size: 90%;">MessageDefinition.event</td>
		<td style="font-size: 90%;"></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-MessageEvent}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-MessageEvent}}</td>
		<td>{{pagelink:DataStandardsWales-MessageHeader}}</td>
		<td style="font-size: 90%;">MessageHeader.event</td>
		<td style="font-size: 90%;"></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-OrganizationClassification}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-OrganizationClassification}}</td>
		<td>{{pagelink:DataStandardsWales-Organization}}</td>
		<td style="font-size: 90%;">Organization.type:classification</td>
		<td style="font-size: 90%;">Embedded in<br> {{pagelink:ValueSet-DataStandardsWales-OrganizationTypeExtended}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-OrganizationDomain}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-OrganizationDomain}}</td>
		<td>{{pagelink:DataStandardsWales-Organization}}</td>
		<td style="font-size: 90%;">Organization.type:domain</td>
		<td style="font-size: 90%;">Embedded in<br> {{pagelink:ValueSet-DataStandardsWales-OrganizationTypeExtended}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-OrganizationSector}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-OrganizationSector}}</td>
		<td>{{pagelink:DataStandardsWales-Organization}}</td>
		<td style="font-size: 90%;">Organization.type:sector</td>
		<td style="font-size: 90%;">Embedded in<br> {{pagelink:ValueSet-DataStandardsWales-OrganizationTypeExtended}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-OrganizationSubclassification}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-OrganizationSubclassification}}</td>
		<td>{{pagelink:DataStandardsWales-Organization}}</td>
		<td style="font-size: 90%;">Organization.type:subclassification</td>
		<td style="font-size: 90%;">Embedded in<br> {{pagelink:ValueSet-DataStandardsWales-OrganizationTypeExtended}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-PatientRecordType}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-PatientRecordType}}</td>
		<td></td>
		<td style="font-size: 90%;"></td>
		<td style="font-size: 90%;">Not bound to profile</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns}}</td>
		<td style="font-size: 90%;">Observation.extension:recordingSetting</td>
		<td style="font-size: 90%;"></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BMI}}</td>
		<td style="font-size: 90%;">Observation.extension:recordingSetting</td>
		<td style="font-size: 90%;"></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight}}</td>
		<td style="font-size: 90%;">Observation.extension:recordingSetting</td>
		<td style="font-size: 90%;"></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-RecordingSetting}}</td>
		<td>{{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight}}</td>
		<td style="font-size: 90%;">Observation.extension:recordingSetting</td>
		<td style="font-size: 90%;"></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-Sex}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-Sex}}</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td style="font-size: 90%;">Patient.extension:birthSex</td>
		<td style="font-size: 90%;">Used for mapping</td>
	</tr>
		<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-Title}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-Title}}</td>
		<td>{{pagelink:DataStandardsWales-Patient}}</td>
		<td style="font-size: 90%;">Patient.name.prefix</td>
		<td style="font-size: 90%;"></td>
	</tr>
		<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-UEC-ActivityType}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-EncounterType}}</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td style="font-size: 90%;">Encounter.type</td>
		<td style="font-size: 90%;"></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-UEC-AttendanceCategory}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-UEC-AttendanceCategory}}</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td style="font-size: 90%;">Encounter.extension:uecAttendanceCategory</td>
		<td style="font-size: 90%;"></td>
	</tr>
		<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-UEC-CareConsultationMechanism}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-EncounterType}}</td>
		<td>{{pagelink:DataStandardsWales-Encounter-UEC}}</td>
		<td style="font-size: 90%;">Encounter.type</td>
		<td style="font-size: 90%;"></td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-UEC-MessageEvent}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-MessageEvent}}</td>
		<td>{{pagelink:DataStandardsWales-MessageDefinition}}</td>
		<td style="font-size: 90%;">MessageDefinition.event</td>
		<td style="font-size: 90%;">DEPRECATED</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-DataStandardsWales-UEC-MessageEvent}}</td>
		<td>{{pagelink:ValueSet-DataStandardsWales-MessageEvent}}</td>
		<td>{{pagelink:DataStandardsWales-MessageHeader}}</td>
		<td style="font-size: 90%;">MessageHeader.event</td>
		<td style="font-size: 90%;">DEPRECATED</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-MessageEvents}}</td>
		<td>{{pagelink:ValueSet-MessageEvents}}</td>
		<td>{{pagelink:DataStandardsWales-MessageDefinition}}</td>
		<td style="font-size: 90%;">MessageDefinition.event</td>
		<td style="font-size: 90%;">Embedded in {{pagelink:ValueSet-DataStandardsWales-MessageEvent}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-MessageEvents}}</td>
		<td>{{pagelink:ValueSet-MessageEvents}}</td>
		<td>{{pagelink:DataStandardsWales-MessageHeader}}</td>
		<td style="font-size: 90%;">MessageHeader.event</td>
		<td style="font-size: 90%;">Embedded in {{pagelink:ValueSet-DataStandardsWales-MessageEvent}}</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-WPASAdmitSource}}</td>
		<td>{{pagelink:ValueSet-PASAdmitSource}}</td>
		<td></td>
		<td style="font-size: 90%;"></td>
		<td style="font-size: 90%;">For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-WPASEventType}}</td>
		<td>{{pagelink:ValueSet-PASEventType}}</td>
		<td></td>
		<td style="font-size: 90%;"></td>
		<td style="font-size: 90%;">For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-WPASReferralSource}}</td>
		<td>{{pagelink:ValueSet-PASReferralSource}}</td>
		<td></td>
		<td style="font-size: 90%;"></td>
		<td style="font-size: 90%;">For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	<tr>
		<td scope="row">{{pagelink:CodeSystem-WPASSourceAdmission}}</td>
		<td>{{pagelink:ValueSet-PASSourceAdmission}}</td>
		<td></td>
		<td style="font-size: 90%;"></td>
		<td style="font-size: 90%;">For CDR/ NHS App use only and not bound to a profile in the IG</td>
	</tr>
	</tbody>
</table>
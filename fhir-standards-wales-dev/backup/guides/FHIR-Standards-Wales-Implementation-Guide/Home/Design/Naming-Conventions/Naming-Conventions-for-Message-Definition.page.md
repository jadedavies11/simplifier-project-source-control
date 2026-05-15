### {{page-title}}

The **logical id** of the resource shall be in the form **DataStandardsWales-[BusinessName]** e.g.
* DataStandardsWales-PatientAdmissionSubmit
* DataStandardsWales-AllergyListUpdate

The **URL** of the resource shall be in the form
**[base URL]/MessageDefinition/DataStandardsWales-[BusinessName]** e.g.
* ```https://fhir.nhs.wales/MessageDefinition/DataStandardsWales-PatientAdmissionSubmit```
* ```https://fhir.nhs.wales/MessageDefinition/DataStandardsWales-AllergyListUpdate```
 
The **name** of the resource - specifically the name.value.element - shall be in the form **DataStandardsWales[BusinessName]** e.g.
* DataStandardsWalesPatientAdmissionSubmit
* DataStandardsWalesAllergyListUpdate
 
The **title** of the resource shall follow the name.value.element, using title case e.g.
* Data Standards Wales Patient Admission Submit
* Data Standards Wales Allergy List Update
 
The **filename** of the resource shall be in the form **[ResourceType]-DataStandardsWales-[BusinessName]** e.g.
* MessageDefinition-DataStandardsWales-PatientAdmissionSubmit
* MessageDefinition-DataStandardsWales-AllergyListUpdate

_Where possible **[BusinessName]** shall be in the form **[MessageEventCode]-[Qualifier]**, with the message event code represented as [UpperCamelCase](https://en.wikipedia.org/wiki/Camel_case). The qualifier is only required when a message event is represented by multiple message definitions for different use cases._

<br><br>

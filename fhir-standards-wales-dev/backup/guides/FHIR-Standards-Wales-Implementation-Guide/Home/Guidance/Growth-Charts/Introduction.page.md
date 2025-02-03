# {{page-title}}

<div style="float:right;border:1px;border-style:solid;padding:10px;margin:10px;width:300px;">

  - [Data Model Overview](#data-model-overview)
  - [FHIR Resources](#fhir-resources)
    * [Encounter](#encounter)
    * [Observation](#observation)
    * [Observation - Vital Signs](#observation-vital-signs)
    * [Practitioner Role](#practitioner-role)
    * [Questionnaire](#questionnaire)
    * [QuestionnaireResponse](#questionnaireresponse)
    * [Related Person](#related-person)
  - [Measures taken by parents or carers](#measures-taken-by-parents-carer)
  - [Use of QuestionnaireResponse instead of Condition](#use-of-questionnaireresponse-instead-of-condition)
</div>

## Data Model Overview
The Growth Chart project utilises FHIR resources to streamline the collection of paediatric growth data. The charts include key parameters such as height, weight, BMI, head circumference, bone age, and certain conditions.
Specific profiles have been developed to represent growth-related observations and administrative details, such as encounters or practitioner roles.

The diagram below provides an overview of the required FHIR resources and how they are interconnected.

The FHIR data model consists of the following resources: 
* {{pagelink:DataStandardsWales-Encounter,text:Encounter}} 
* {{pagelink:DataStandardsWales-Observation,text:Observation}}
* {{pagelink:DataStandardsWales-Observation-VitalSigns,text:Observation-Vital Signs}}
* {{pagelink:DataStandardsWales-Observation-VitalSigns-BMI,text:Observation-Vital Signs-BMI}}
* {{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight,text:Observation-Vital Signs-Body Height}}
* {{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight,text:Observation-Vital Signs-Body Weight}}
* {{pagelink:DataStandardsWales-Patient,text:Observation}}
* {{pagelink:DataStandardsWales-Practitioner,text:Practitioner}}
* {{pagelink:DataStandardsWales-PractitionerRole,text:Practitioner Role}}
* {{pagelink:DataStandardsWales-Questionnaire,text:Questionnaire}}
* {{pagelink:DataStandardsWales-QuestionnaireResponse,text:Questionnaire Response}}
* {{pagelink:DataStandardsWales-RelatedPerson,text:Related Person}}


<br>

{{render:Diagrams-growth-chart-simplified-logical-model}}

<br />


## FHIR Resources

### Encounter
The {{pagelink:DataStandardsWales-Encounter,text:Data Standards Wales Encounter Profile}} represents a patient's attendance or meeting with a healthcare professional, often in a healthcare facility (although it can also include domiciliary visits). 

To link a growth chart measurement event to a specific encounter, the `Encounter.class` has been linked to a SNOMED code for Growth Chart (record artifact).

### Observation - Vital Signs

The Observation - Vital Signs profile and its children, are used for specific observations linked to measurements taken from the patient or someone related to the patient. In the context of growth charts, it includes the following:

* {{pagelink:DataStandardsWales-Observation-VitalSigns,text:Data Standards Wales Observation-Vital Signs Profile}} - included here is Head Circumference.
  * {{pagelink:DataStandardsWales-Observation-VitalSigns-BMI,text:Data Standards Wales Observation-Vital Signs-BMI Profile}}
  * {{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight,text:Data Standards Wales Observation-Vital Signs-Body Height Profile}}  - including that of the parents of the child
  * {{pagelink:DataStandardsWales-Observation-VitalSigns-BodyWeight,text:Data Standards Wales Observation-Vital Signs-Body Weight Profile}}


### Observation 
{{pagelink:DataStandardsWales-Observation,text:Data Standards Wales Observation Profile}} is for any other observation that is not considered a vital sign. We have, in this context, Bone Age, which is a parameter or measure taken from an X-Ray and not from the patient themselves. 

Bone age has then been classified as an `Observation` resource with `Observation.category` of "Imaging".

<br>

{{render:Diagrams-LogicalModel-growthChart-ObservationGroup}}

<br />


### Practitioner
A {{pagelink:DataStandardsWales-Practitioner,text:Practitioner}} in FHIR is any health and care professional that is involved in the care of a patient or citizen. 

In many cases, healthcare professionals without a professional registration (e.g., Healthcare Support Workers) may take measurements, make observations, and author documentation. For these users, there is an option to capture their Nadex as part of `Practitioner.identifier`.
{{pagelink:DataStandardsWales-PractitionerRole,text:Data Standards Wales Practitioner Role}}

### Questionnaire
{{pagelink:DataStandardsWales-Questionnaire,text:Data Standards Wales Questionnaire Profile}} is used here to capture information about the patient's condition (currently either Turner's or Down syndrome). 


### QuestionnaireResponse
Each time a user selects a type of patient condition, an instance conforming to the {{pagelink:DataStandardsWales-QuestionnaireResponse,text:Data Standards Wales Questionnaire Response Profile}} is created, which is linked to the corresponding {{pagelink:DataStandardsWales-Questionnaire,text:Questionnaire}}. 

The QuestionnaireResponse contains information about notable patient conditions, such as Down syndrome or Turner syndrome. If neither condition is selected, the default response is UK WHO. This selection determines which graph is presented to the user for plotting measurements.


### Related Person
A {{pagelink:DataStandardsWales-RelatedPerson,text:Related Person}} could be anyone connected to the patient. In this case, it is particularly relevant for parents or carers of the child, as they may occasionally provide data for the growth chart.

The role of {{pagelink:DataStandardsWales-RelatedPerson,text: Data Standards Wales Related Person Profile}} is also significant when referencing Mid-Parental Height. This measure, derived from the natural mother’s and natural father’s heights, uses the {{pagelink:DataStandardsWales-Observation-VitalSigns-BodyHeight,text:Data Standards Wales Observation-Vital Signs-Body Height Profile}} as the base. Here, the `subject` is the patient (i.e., the child), and the `focus` is set to the 'natural mother' or 'natural father'.

<br>

{{render:Diagrams-LogicalModel-growthChart-MidParentalHeight}}

<br />

## Measures taken by parents or carers
A child’s height or weight may be measured by parents or carers who have received training from healthcare professionals. It is important to capture this on the form, as the author of the form might be a healthcare professional, but the `Observation.performer` for a specific measurement would reference {{pagelink:DataStandardsWales-RelatedPerson,text: a Related Person}}.

## Use of QuestionnaireResponse instead of Condition
At this stage, insufficient data is available to create a definitive condition list. For instance, Down syndrome or Turner syndrome might be recorded during form completion, but key details such as the author, date of diagnosis, and verification status are not captured (currently only provisionally marked and unconfirmed by a clinician).

Additionally, these terms are too broad and do not differentiate between subtypes (e.g., complete trisomy 21 vs mosaic trisomy 21), each requiring separate SNOMED CT codes. This granularity is unavailable at this point.

Our recommendation is to use a {{pagelink:DataStandardsWales-Questionnaire,text:Questionnaire}} and a {{pagelink:DataStandardsWales-QuestionnaireResponse,text:Questionnaire Response}} to record the information for now. A more comprehensive condition record can be developed in the future, where data is maintained by the appropriate clinician and updated as needed. Mapping will also be required in later stages.



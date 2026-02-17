## Submission of UEC data to the CDR
### FHIR Messaging Resources
Submissions of UEC data from UEC applications to the CDR will use the FHIR messaging paradigm and the following FHIR messaging resources:
* [Bundle](https://www.hl7.org/fhir/R4/bundle.html) 
* {{pagelink:DataStandardsWales-MessageDefinition, text:MessageDefinition}}
* {{pagelink:DataStandardsWales-MessageHeader, text:MessageHeader}}

The following resource will be used within the response bundle to convey any issues encountered by the CDR message handler:
* [OperationOutcome](https://www.hl7.org/fhir/R4/operationoutcome.html)

See the dedicated guidance page for clarification of the purpose and use of the resources involved in FHIR messaging: {{pagelink:Home/Guidance/FHIR-Messaging/Index.page.md, text: FHIR Messaging Guidance}}

### UEC Message Events
The following message events have been defined FOR TRIAL USE at Phase 1, pending the establishment of a naming convention for message events.

| Message event | Submission point             | Resources (if applicable to use case)           |
|:--|:--|:------|
| uec-arrival<br /><br /><br /><br /><br /><br /> | On completion of registering the <br />patient’s arrival at the UEC facility<br /><br /><br /><br /><br /> | UEC Encounter <br />Patient<br />Organization (service provider)<br />Organization (attendance source)<br />Organization (managing UEC facility)<br />Location (UEC facility) |
| uec-triage<br /><br /><br /><br /><br /><br /><br /><br /><br /> | On completion of recording the <br />triage assessment<br /><br /><br /> <br /><br /><br /><br /><br /> | UEC Encounter <br />Patient<br />Organization (service provider)<br />Organization (attendance source)<br />Organization (managing UEC facility)<br />Location (UEC facility)<br />ProfessionalRole (e.g. triage nurse)<br />Condition (chief complaint)<br />Condition (each comorbidity) |
| uec-discharge<br /><br /><br /><br /><br /><br /><br /><br /><br /> | On completion of the UEC attendance <br />i.e. the point of discharge<br /><br /><br /><br /><br /><br /><br /><br /> | UEC Encounter <br />Patient<br />Organization (service provider)<br />Organization (attendance source)<br />Organization (managing UEC facility)<br />Location (UEC facility)<br />ProfessionalRole (each professional)<br />Condition (chief complaint)<br />Condition (each comorbidity) |

These message events have been captured in a dedicated code system that can be extended as the scope increases through the project phases:
* {{pagelink:CodeSystem-DataStandardsWales-UEC-MessageEvent}}

### UEC Message Definitions
MessageDefinition resource instances have been defined FOR TRIAL USE for the Phase 1 UEC data submissions
* {{pagelink:MessageDefinition-DataStandardsWales-UEC-Arrival}}
* {{pagelink:MessageDefinition-DataStandardsWales-UEC-Triage}}
* {{pagelink:MessageDefinition-DataStandardsWales-UEC-Discharge}}
<br />
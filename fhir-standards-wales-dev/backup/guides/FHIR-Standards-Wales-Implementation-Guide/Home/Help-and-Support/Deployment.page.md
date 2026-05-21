## {{page-title}}

### Dependencies

This FHIR project has a basic dependency on HL7 FHIR R4. Project dependencies may change according to specific local requirements.

Dependencies enable synchronisation with the packages they are derived from without the need to add separate files and incur additional maintenance.

To support a common approach to the creation and maintenance of HL7 FHIR standards across the four nations, the Data Standards Wales FHIR package also contains resources derived from HL7 FHIR UK Core where these exist.

To enable backporting of data from HL7 FHIR R5 into HL7 FHIR R4 in a standardised way, the Data Standards Wales FHIR package also has a dependency on the hl7.fhir.uv.xver-r5.r4 package. The majority of FHIR implementations within NHS Wales are based on HL7 FHIR R4 and the dependency on hl7.fhir.uv.xver-r5.r4 allows us to use HL7 FHIR R5 resources without the need to upgrade to that release as base.  

A history of dependencies used in the Data Standards Wales FHIR package can be found in the Dependencies History section of our [Version History IG](https://simplifier.net/guide/Wales-FHIR-Implementation-Guide-Version-History/) page.

Please ensure that you have downloaded the relevant dependencies when implementing the Data Standards Wales FHIR profiles into your system.

#### Model
The draft diagram below illustrates the relationship between Data Standards Wales FHIR packages and their dependencies.
{{render:Diagrams-Guidance-Dependencies}}

#### Backport Extensions
Dependency on the HL7 FHIR backport extension enables Data Standards Wales FHIR Profiles, which are based on HL7 FHIR R4 standards, to include elements from HL7 FHIR R5. 
{{pagelink:Home/FHIR-Assets/Backport-Extensions.page.md, text: Backport Extensions}} provides a list of HL7 FHIR R5 extension elements used in the Data Standards Wales FHIR package along with the profiles they are bound to.  

#### Firely Terminal

The Firely Terminal includes all necessary packages for your system implementation but requires a Firely licence to use commercially.  This can, however, be used for testing purposes.

#### NPM

Ensure that you download each package individually so that all asset dependencies are available.

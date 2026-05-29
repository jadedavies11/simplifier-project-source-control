## {{page-title}}

### Dependencies

The Wales FHIR Implementation Guide is a specialisation of the HL7 FHIR R4 standard containing tailored profiles and related FHIR assets for use within NHS Wales. FHIR package dependencies enable synchronisation with the packages they are derived from without the need to add separate files and incur additional maintenance. Where projects further specialise the Wales FHIR standard, they may add dependencies according to specific local requirements.

This FHIR project has the following dependencies:

* A basic dependency on HL7 FHIR R4
* A dependency on HL7 FHIR UK Core to support a common approach to HL7 FHIR standards across the four nations
* A dependency on hl7.fhir.uv.xver-r5.r4 to support the backporting of elements not introduced until HL7 FHIR R5

These FHIR package dependencies are illustrated below. Note that the illustration for HL7 FHIR UK Core depicts an anticipated future dependency on hl7.fhir.uv.xver-r5.r4xver and is not a statement of the current dependencies in fhir.r4.ukcore.stu2 2.0.1.

{{render:Diagrams-Guidance-Dependencies}}


In creating profiles for NHS Wales the HL7 FHIR UK Core profiles are used as the base for specialisation where these exist for the specific resource type. In the absence of UK Core profiles, the Wales profiles are based directly upon HL7 FHIR resources. A similar priority order applies to the use of extensions. Where no suitable HL7 FHIR UK Core extension exists nor any suitable HL7 extension, then the resource definition is checked for an applicable new element in HL7 FHIR R5 or R6, ensuring that the appropriate cross-version backport package dependency is established to support the use of the backport extension. If there is no suitable backport option, then a Wales-specific extension may be considered.  

A history of dependencies used in the Data Standards Wales FHIR package can be found in the Dependencies History section of our [Version History IG](https://simplifier.net/guide/Wales-FHIR-Implementation-Guide-Version-History/) page.

<b>Please ensure that you have downloaded the relevant dependencies when implementing the Data Standards Wales FHIR profiles into your system.</b>


#### Backport Extensions
Dependency on the HL7 FHIR cross version R5 to R4 backport extension package enables Data Standards Wales FHIR Profiles, which are based on HL7 FHIR R4 standards, to include elements from HL7 FHIR R5. 
{{pagelink:Home/FHIR-Assets/Backport-Extensions.page.md, text: Backport Extensions}} provides a list of HL7 FHIR R5 extension elements used in the Data Standards Wales FHIR package along with the profiles they are bound to.  

#### Firely Terminal

The Firely Terminal includes all necessary packages for your system implementation but requires a Firely licence to use commercially.  This can, however, be used for testing purposes.

#### NPM (Node Package Manager)

Ensure that you download each package individually so that all asset dependencies are available.

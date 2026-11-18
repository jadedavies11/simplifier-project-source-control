## {{page-title}}

### Release Strategy

Following on from a Discovery phase in 2022/23, an initial Standard for Trial Use 1 (STU1) was balloted in early 2023, followed by Standard for Trial Use 2 (STU2) in late 2024. Full details of the releases and versions of the NHS Wales FHIR Standards can be found on the NHS Wales [FHIR Implementation Guide Version History](https://simplifier.net/guide/wales-fhir-implementation-guide-version-history/) Site.

This release strategy follows the [UK Core Publication History](https://simplifier.net/guide/ukcoreversionhistory?version=current).

### Balloting and Change Management

Following the STU1 and STU2 ballot releases, we are developing a review strategy to obtain feedback on profiles in partnership with the Interoperability Standards Working Group, including balloted review of minor versions. Full release notes of all previous changes can be found on the {{pagelink:Release-Notes}} page of this Implementation Guide.

### Release Status

Standards for Trial Use (STU) is a term used to describe a package release as opposed to its constituent resources. The term STU is usually suffixed with a number to denote the current version (e.g. STU1, STU2, etc.) and the number will increase.

A STU release is relatively stable, insofar as it has been though the NHS Wales FHIR Standards Development Process and, depending on the types of change, may have culminated in the NHS Wales FHIR Ballot Process.

It should be noted that HL7 and UK Core, who provide the base profiles our project uses, both have their own STU numbering. These and our own releases, therefore, have three separate STU numbering sequences that are not interchangeable. Please ensure that the correct STU sequence is being referenced depending on the release and provider.

### Resource Status

This denotes the [publication status](https://build.fhir.org/codesystem-publication-status.html) of the resources within the release and reflects the lifecycle stage of the **standard**.  

|Status|Definition|Environments|Experimental| 
|--|--|--|--|
|<span style="background-color:orange;color:white;">**Draft**</span>|This resource is authored for testing purposes only and is not intended for progression to production. It enables experimental content to be developed following the same lifecycle that would be used for a production-level structure definition.|Development<br>Test|<span style="background-color:red;color:white">**Experimental**</span>|
|<span style="background-color:orange;color:white;">**Draft**</span> |This resource is still under development and is not yet considered to be ready for normal use. It may have known issues or still be in the "in development" stage. It is included in the production environment for review or to solicit feedback from the implementation community. It is not recommended for production use and implementation is "use at your own risk".| Development<br>Test<br>Production |No|
|<span style="background-color:green;color:white">**Active**</span>| This resource has been subjected to ballot and approved as a standard. It is considered by the authors to be ready for use in production systems, however it may not yet have seen widespread use in production across the full spectrum of environments as is intended. In some cases, there may be documented known issues that require implementation experience to determine appropriate resolutions.|Development<br>Test<br>Production|No|
|<span style="background-color:grey;color:white">**Retired**</span>|This resource has been withdrawn or superseded and should no longer be used. Implementers who already support it should continue to do so for backward compatibility. It should not be used in new implementations. Where a resource is categorised as Retired there will be additional guidance on what to use as an alternative.|Development<br>Test<br>Production|No| 

As Resource Status reflects the lifecycle stage of the standard, the status may change across versions to reflect typical development progression e.g. Draft to Active. Where a resource is Active and its contents are then changed, for example introduction of a new element, the Resource Status does not revert to Draft as this would imply that the resource is no longer considered ready for use in production systems, which would be extremely rare. The decision to 'downgrade' a status from Active would only be considered where the resource is fundamentally flawed and in such examples the decision may be made to Retire that resource rather than change to Draft. 

The Resource Status is used for all resources where we include version data, including: 

- Profiles
- Extensions
- Value Sets
- Code Systems
- Concept Maps
- Message Definitions

**Note** - For Value Sets and Code Systems the Resource Status reflects the status of the Value Set or Code System itself, and not the values contained within, which may be subject to change. 

**Note** - HL7 FHIR applies additional terminology to denote the stability of its standards ([Standard Status](https://build.fhir.org/versions.html#std-process)) and how widely the standards have been tested and adopted ([FHIR Maturity Level](https://build.fhir.org/versions.html#maturity)). This level of detail is not utilised in the Wales FHIR Implementation Guide.

### Profile Maturity

Active profiles can be used for implementation and we would encourage anyone beginning development to inform the InterOp Delivery Team so that assistance can be provided. This will also be used as an opportunity to review and influence the content in the implementation guide.

Active profiles have been scrutinised by the Interoperability Working Group FHIR Task & Finish group and ballot process. While the profiles are designed to have some rigidity, the intention is for development to be flexible to the needs of system owners throughout NHS Wales. Development of these assets will continue in future iterations and as they increase in maturity the number of expected changes will decrease.

Draft assets may change regularly and should not be expected to remain more stable until an active version is published. It is recommended that implementors looking to utilise these profiles should only do so for testing purposes. Individuals are encouraged to engage in the development of these profiles to ensure they are fit for purpose. The inclusion of a draft asset does not guarantee it will become active in a future release and, while unlikely, they may be removed following consultation with key stakeholders.


# Wales FHIR Implementation Guide v0.1.1 STU1 - for ballot

<div class="warning">
<p><b>Important:</b>This is the v1.0 Standard for Trial use (STU1) release of the Data Standards Wales FHIR Implementation Guide. There is a mixture of active and draft FHIR resources which have been published following the inaugural ballot process. The active profiles have been scrutinised by the FHIR Task & Finish group and they may be developed further in future iterations. Active profiles can be used for implementation and we would encourage anyone beginning development to inform the Interoperability Delivery Team. While the profiles have some rigidity, the intention is for development to be flexible to the needs of system owners throughout NHS Wales.

Some profiles are also provided in an experimental state which have not undergone a more thorough review cycle. The latter are liable to change regularly and should not be expected to remain stable until they move to draft. The assets contained in this implementation guide may not make it to the next major version following the results of balloting.
</div>
<br>

The guidance contains:
* FHIR resource profiles and extensions.
* FHIR terminology components including ValueSets, CodeSystems and ConceptMaps.
* Example FHIR resources.
* Other general guidance useful to FHIR implementers in Wales.

### Project Description and Scope
This Implementation Guide contains the HL7 FHIR R4 standards for use by Health and Care organisations in Wales.
* This is part of the Simplifier [NHS Wales Organisation](https://simplifier.net/organization/nhswales) and the [FHIR Standards Wales Project](https://simplifier.net/fhir-standards-wales).
* These standards are derived from the [UK Core Implementation Guide 1.0.0 - STU1 Release](https://simplifier.net/guide/uk-core-implementation-guide?version=1.0.0).
* Some experimental profiles are derived from the [UK Core Implementation Guide STU2 Release for Ballot](https://simplifier.net/guide/uk-core-implementation-guide-stu2) or [UK Core Assets in Development](https://simplifier.net/guide/UKCoreImplementationGuideAssetsinDevelopment/Home).
* All relevant NHS Wales [Data Standards](https://dhcw.nhs.wales/information-services/information-standards/data-standards/) are implemented.
* The latest package is [fhir.r4.wales.stu1 0.1.1-ballot](https://simplifier.net/packages/fhir.r4.wales.stu1/0.1.1-ballot).
* Our GitHub page can be found here [NHSWalesFHIR/NHSWales-fhir-profiles-R4](https://github.com/NHSWalesFHIR/NHSWales-fhir-profiles-R4)
* Further versions of this guide will be published once the UK Core ballot process is concluded. These will be subject to assurance by the Welsh Technical Standards Board.
* Please see the [UK Core version history](https://simplifier.net/guide/ukcoreversionhistory) guide for insight into future UK Core releases.

<div class="warning"><span class="ExtLinkWarn"></span></div>

### Resource Index
|People|Entities|Workflow|
|-
|{{pagelink:DataStandardsWales-Patient}}|{{pagelink:DataStandardsWales-Organization}}|{{pagelink:DataStandardsWales-Encounter}} <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span></div>|
|{{pagelink:DataStandardsWales-Practitioner}} |{{pagelink:DataStandardsWales-Location}}||
|{{pagelink:DataStandardsWales-PractitionerRole}}||

<!---->
|Diagnostics|Medications|Allergy|
|-
|{{pagelink:DataStandardsWales-ServiceRequest}} <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span>| {{pagelink:DataStandardsWales-Medication}}|{{pagelink:DataStandardsWales-AllergyIntolerance}}|
|{{pagelink:DataStandardsWales-DiagnosticReport}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span> |{{pagelink:DataStandardsWales-MedicationAdministration}}|{{pagelink:DataStandardsWales-AllergyList}}|
|{{pagelink:DataStandardsWales-DiagnosticReport-Lab}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span> | {{pagelink:DataStandardsWales-MedicationDispense}}||
|{{pagelink:DataStandardsWales-Observation}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span> | {{pagelink:DataStandardsWales-MedicationList}}||
|{{pagelink:DataStandardsWales-Observation-Lab}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span>  |{{pagelink:DataStandardsWales-MedicationRequest}}||
|{{pagelink:DataStandardsWales-Specimen}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span>  |{{pagelink:DataStandardsWales-MedicationStatement}}||
|{{pagelink:DataStandardsWales-ImagingStudy}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span>  |{{pagelink:DataStandardsWales-Dosage}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span></div>||
|{{pagelink:DataStandardsWales-Endpoint}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span>  |{{pagelink:DataStandardsWales-Immunization}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span></div>|


### Related Pages

<div class="container">
    <div class="row">
        <div class="col-md-7 card">
            <h4><b><a href="https://simplifier.net/guide/uk-core-implementation-guide?version=1.0.0" alt="UK Core Implementation Guide 1.0.0 - STU1 Release for Ballot" target="_blank">UK Core v1.0.0 STU1 Implementation Guide</a></b></h4>
            <p>UK Core v1.0.0 STU1 Implementation Guide</p>
        </div>
        <div class="col-md-7 card">
            <h4><b><a href="https://simplifier.net/guide/uk-core-implementation-guide-stu2" alt="UK Core Implementation Guide STU2 Release for Ballot" target="_blank">UK Core STU2 Implementation Guide</a></b></h4>
            <p>UK Core STU2 Implementation Guide</p>
        </div>
        <div class="col-md-7 card">
            <h4><b><a href="https://build.fhir.org/ig/HL7-UK/UK-Core-Access/index.html" alt="UK Core Access" target="_blank">UK Core Access Implementation Guide</a></b></h4>
            <p>Specifies the requirements for a RESTful endpoint providing read-only access for direct care and subject of care access</p>
        </div>
        <div class="col-md-7 card">
            <h4><b><a href="https://simplifier.net/guide/ukcoreversionhistory" alt="UK Core Version History" target="_blank">UK Core Version History</a></b></h4>
            <p>Reference point for published and development versions of the UK Core</p>
        </div>
        <div class="col-md-7 card">
            <h4><b><a href="https://simplifier.net/guide/UKCoreImplementationGuideAssetsinDevelopment/Home" alt="UK Core Assets in Development" target="_blank">UK Core Assets in Development</a></b></h4>
            <p>Assets currently in development for UK Core</p>
        </div>
    </div>
</div>
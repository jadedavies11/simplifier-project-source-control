# Wales FHIR Implementation Guide v0.1.1 STU1 - for ballot

<div class="warning">
<p><b>Important:</b> This is the initial v0.1.1 Standard for Trial use (STU1) release of the Data Standards Wales FHIR Implementation Guide for ballot. This version contains a minimal number of base FHIR resources and should be considered 'under development' and should NOT be implemented until the first major version is released (v1.0.0). As a major version has not yet been published it should not be used in production systems. This has been published in order to support development with stakeholders via a ballot mechanism and for comment and feedback.
<p>This project currently contain draft profiles that have undergone a first pass review.  Some profiles are also provided in an experimental state which have not undergone a more thorough review cycle. The latter are liable to change regularly and should not be expected to remain stable until they move to draft. The assets contained in this implementation guide may not make it to the next major version following the results of balloting. 
</div>

### Project Description and Scope
This Implementation Guide contains the HL7 FHIR R4 standards for use by Health and Care organisations in Wales.
* This is part of the Simplifier [NHS Wales Organisation](https://simplifier.net/organization/nhswales) and the [FHIR Standards Wales Project](https://simplifier.net/fhir-standards-wales).
* These standards are derived from the [UK Core Implementation Guide 1.0.0 - STU1 Release](https://simplifier.net/guide/uk-core-implementation-guide?version=1.0.0).
* Some experimental profiles are derived from the [UK Core Implementation Guide STU2 Release for Ballot](https://simplifier.net/guide/uk-core-implementation-guide-stu2?version=current) or [UK Core Assets in Development](https://simplifier.net/guide/UKCoreImplementationGuideAssetsinDevelopment/Home?version=current).
* All relevant NHS Wales [Data Standards](https://dhcw.nhs.wales/information-services/information-standards/data-standards/) are implemented.
* The latest package is [fhir.r4.wales.stu1 0.1.1-ballot](https://simplifier.net/packages/fhir.r4.wales.stu1/0.1.1-ballot).
* Our GitHub page can be found here [NHSWalesFHIR/NHSWales-fhir-profiles-R4](https://github.com/NHSWalesFHIR/NHSWales-fhir-profiles-R4)
* Further versions of this guide will be published once the UK Core ballot process is concluded. These will be subject to assurance by the Welsh Technical Standards Board.
* Please see the [UK Core version history](https://simplifier.net/guide/ukcoreversionhistory?version=current) guide for insight into future UK Core releases.

The guidance contains:
* FHIR resource profiles and extensions.
* FHIR terminology components including ValueSets, CodeSystems and ConceptMaps.
* Example FHIR resources.
* Other general guidance useful to FHIR implementers in Wales.



### Resource Index
|People|Entities|Workflow|
|-
|{{pagelink:DataStandardsWales-Patient}} <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a> |{{pagelink:DataStandardsWales-Organization}} <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a>|{{pagelink:DataStandardsWales-Encounter}} <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span></div>|
|{{pagelink:DataStandardsWales-Practitioner}} <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a> |{{pagelink:DataStandardsWales-Location}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a> ||
|{{pagelink:DataStandardsWales-PractitionerRole}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a> ||

<!---->
|Diagnostics|Medications|Allergy|
|-
|{{pagelink:DataStandardsWales-ServiceRequest}} <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span>| {{pagelink:DataStandardsWales-Medication}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a> |{{pagelink:DataStandardsWales-AllergyIntolerance}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a>|
|{{pagelink:DataStandardsWales-DiagnosticReport}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span> |{{pagelink:DataStandardsWales-MedicationAdministration}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a>|{{pagelink:DataStandardsWales-AllergyList}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a>|
|{{pagelink:DataStandardsWales-DiagnosticReport-Lab}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span> | {{pagelink:DataStandardsWales-MedicationDispense}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a> ||
|{{pagelink:DataStandardsWales-Observation}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span> | {{pagelink:DataStandardsWales-MedicationList}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a>||
|{{pagelink:DataStandardsWales-Observation-Lab}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span>  |{{pagelink:DataStandardsWales-MedicationRequest}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a>||
|{{pagelink:DataStandardsWales-Specimen}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a><div class="tagexperimental tt">E<span class="tooltiptext">Experimental profile</span>  |{{pagelink:DataStandardsWales-MedicationStatement}}  <a href="/ui/workflow/overview?id=1" class="tagdraft" target="_blank">Draft</a>||
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
            <h4><b><a href="https://simplifier.net/guide/uk-core-implementation-guide-stu2?version=current" alt="UK Core Implementation Guide STU2 Release for Ballot" target="_blank">UK Core STU2 Implementation Guide</a></b></h4>
            <p>UK Core STU2 Implementation Guide</p>
        </div>
        <div class="col-md-7 card">
            <h4><b><a href="https://build.fhir.org/ig/HL7-UK/UK-Core-Access/index.html" alt="UK Core Access" target="_blank">UK Core Access Implementation Guide</a></b></h4>
            <p>Specifies the requirements for a RESTful endpoint providing read-only access for direct care and subject of care access</p>
        </div>
        <div class="col-md-7 card">
            <h4><b><a href="https://simplifier.net/guide/ukcoreversionhistory?version=current" alt="UK Core Version History" target="_blank">UK Core Version History</a></b></h4>
            <p>Reference point for published and development versions of the UK Core</p>
        </div>
        <div class="col-md-7 card">
            <h4><b><a href="https://simplifier.net/guide/UKCoreImplementationGuideAssetsinDevelopment/Home?version=current" alt="UK Core Assets in Development" target="_blank">UK Core Assets in Development</a></b></h4>
            <p>Assets currently in development for UK Core</p>
        </div>
    </div>
</div>
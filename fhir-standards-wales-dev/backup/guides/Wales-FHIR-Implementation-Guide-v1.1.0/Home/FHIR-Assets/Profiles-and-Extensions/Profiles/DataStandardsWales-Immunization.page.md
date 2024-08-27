<div class="warning"><span class="ExperiWarn"></span></div>

## {{page-title}}

### FQL

@```
    from
        StructureDefinition
    where
        name='DataStandardsWalesImmunization'
    select 
        Profile: name,
        Type: type,
        Status: status,
        Canonical: url
```

The [Immunization](https://www.hl7.org/fhir/r4/immunization.html) resource is a record of the immunization received by a patient.

The {{page-title}} profile is derived from the [UK Core Immunization Profile](https://simplifier.net/guide/uk-core-implementation-guide/Home/ProfilesandExtensions/ProfileUKCore-Immunization?version=1.0.0). It defines additional rules for use within health and care organisations in Wales.

A direct link to the Data Standards Wales asset can be accessed here - {{link:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Immunization}}

### Formal Views of Profile Content
<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink tab-active" onclick="openCity(this,'tabsnap')" data-target="tabsnap">
      Snapshot View
    </li>
    <li class="tablink" onclick="openCity(this,'tabdiff')" data-target="tabdiff">
      Differential View
    </li>
    <li class="tablink" onclick="openCity(this,'tabhybrid')" data-target="tabhybrid">
      Hybrid View
    </li>
    <li class="tablink" onclick="openCity(this,'tabeg')" data-target="tabeg">
      Examples
    </li>    
  </ul>
  <div class="tab-main">
    <div id="tabsnap" class="tabcontent active">      
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Immunization, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Immunization, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Immunization, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>Currently under development</li> 
    </list>
  </div>    
</div>

---

### Example Usage Scenarios ###
The following are example usage scenarios for the Immunisation profile:

- <add link to example> Query for a Flu Vaccination using the query parameter `Immunization.vaccineCode` to specify which vaccine product has been administered.
- <add link to example> Query for a vaccine that wasn't given using query parameters such as `Immunization.status` and `Immunization.statusReason` and .
- <add link to example> Query for the dosage of an Oral Solution PRN medication using query parameters such as `Dosage.asNeededCodeableConcept` and `Dosage.doseAndRate.doseRange`.

_*Examples provided have been clinically assured on the 07-Aug-2024_

---

### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Home/Introduction/Profile-Descriptions/Mandatory-and-Must-Support-Data-Elements.page.md,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.

Each Immunization must have:
1. status
2. vaccineCode
3. patient
4. occurance

Each Immunization must support:
1. identifier
2. statusReason
3. recorded
4. reportOrigin
5. location
6. manufacturer
7. lotNumber
8. expirationDate
9. site
10. route
11. doseQuantity
12. performer
13. reasonCode
14. protocolApplied
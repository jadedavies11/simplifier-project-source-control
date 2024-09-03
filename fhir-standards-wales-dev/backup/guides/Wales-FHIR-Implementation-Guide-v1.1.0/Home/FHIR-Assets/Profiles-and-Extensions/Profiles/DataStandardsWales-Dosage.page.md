---
name: DataStandardsWalesPatient
---

<div class="warning"><span class="ExperiWarn"></span></div>

## {{page-title}}

### FQL

@```
    from
        StructureDefinition
    where
        name='DataStandardsWalesDosage'
    select 
        Profile: name,
        Type: type,
        Status: status,
        Canonical: url
```

The [Dosage](https://www.hl7.org/fhir/r4/dosage.html) resource is a record of a medication that is administered to a patient.

The {{page-title}} profile is derived from the [HL7 Dosage Profile](https://www.hl7.org/fhir/r4/dosage.html). It defines additional rules for use within health and care organisations in Wales.

A direct link to the Data Standards Wales asset can be accessed here - {{link:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Dosage}}

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Dosage, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Dosage, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Dosage, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>under development</li> 
    </list>
  </div>    
</div>


---

### Example Usage Scenarios ###
The following are example usage scenarios for the Dosage profile:

- <add link to example> Query for the dosage of an Eye Drops medication using the query parameter `Dosage.timing.repeat.when` when the time value is undefined.
- <add link to example> Query for the dosage of an Inhaler medication using query parameters such as `Dosage.additionalInstruction`.
- <add link to example> Query for the dosage of an Oral Solution PRN medication using query parameters such as `Dosage.asNeededCodeableConcept` and `Dosage.doseAndRate.doseRange`.

_*Examples provided have been clinically assured on the 07-Aug-2024_

---

## Profile Specific Implementation Guidance: ##


### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Home/Introduction/Profile-Descriptions/Mandatory-and-Must-Support-Data-Elements.page.md,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.

Each Dosage must support:

|Element|Reason|
|-|-|
|`Dosage.sequence`|Indicates the order in which the dosage instructions should be applied or interpreted.|
|`Dosage.text`|Free text that can be used for cases where the instructions are too complex to code.|
|`Dosage.additionalInstruction`|Supplemental instructions or warnings.|
|`Dosage.patientInstruction`|Supplemental instructions to the patient on how to take the medication.|
|`Dosage.timing`|The timing schedule for taking or administering the medication.|
|`Dosage.asNeeded`|It indicates if there is a precondition for taking the medication.|
|`Dosage.site`|Body site to administer to.|
|`Dosage.route`|Indication on how the drug should enter the body.|
|`Dosage.method`|Technique for administering the medication.|
|`Dosage.maxDosePerPeriod`|Upper limit on medication per unit of time.|

---

### `doseAndRate`

By preference, use [UCUM](http://unitsofmeasure.org) for dose units. Examples of these units of measure are “gram” or “milliliter” or “percent”.

Where a UCUM unit of measure is not defined, use a [SNOMED-CT](http://snomed.info/sct).
Examples of when a SNOMED-CT unit of measure would typically be used are “tablet”, “capsule” or “ampule”.

**Recommendation**: Dose is used to specify the quantity of the medication administered and not the strength of the active ingredient. This information will be specified on `Medication.ingredient.strength`,

---



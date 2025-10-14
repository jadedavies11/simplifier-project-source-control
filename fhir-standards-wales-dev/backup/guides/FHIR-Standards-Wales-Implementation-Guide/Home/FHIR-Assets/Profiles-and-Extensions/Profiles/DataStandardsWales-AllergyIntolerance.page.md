<div class="warning"><span class="ImplementWarn"></span></div>

## {{page-title}}

### Overview
The [AllergyIntolerance](https://www.hl7.org/fhir/r4/AllergyIntolerance.html) resource is primarily used to provide a single place with the heath record to document reactions to substance like materials, food or medications. The resource can be used to catalogue reactions to exposures over time including when no reaction takes place at all. The resource can be used to build a catalogue of allergies and intolerances and how they change over time. 

The {{page-title}} profile is derived from the [UK Core AllergyIntolerance Profile](https://simplifier.net/guide/UK-Core-Implementation-Guide-STU2/Home/ProfilesandExtensions/Profile-UKCore-AllergyIntolerance?version=2.0.1). It defines additional rules for use within health and care organisations in Wales.

A direct link to the Data Standards Wales asset can be accessed here - {{link:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-AllergyIntolerance}}

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-AllergyIntolerance, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-AllergyIntolerance, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-AllergyIntolerance, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>{{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/Examples/Allergies/Example-DataStandardsWales-AllergyIntolerance-Potato.page.md, text:Example food allergy - Potato}}</li>
      <li>{{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/Examples/Allergies/Example-DataStandardsWales-AllergyIntolerance-deleted.page.md, text:Example deleted allergy - Potato}}</li> 
      <li>{{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/Examples/Allergies/Example-DataStandardsWales-AllergyIntolerance-NoKnownAllergy.page.md, text:Example exclusion - no known allergy}}</li> 
      <li>{{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/Examples/Allergies/Example-DataStandardsWales-AllergyIntolerance-Aspirin.page.md, text:Example medication allergy -Aspirin}}</li>                 
    </list>
  </div>    
</div>

### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Home/Introduction/Profile-Descriptions/Mandatory-and-Must-Support-Data-Elements.page.md,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.
 
Each AllergyIntolerance must have:
1. A code
1. A patient

Each Encounter must support:
1. A code to indicate clinical status
1. An encounter
1. A recorded date
1. A recorder
1. An asserter
1. Clinical details for reactions recorded for the AllergyIntolerance
1. Evidence *

_*see Implementation Guidance for the evidence extension below_


* The extensions listed below allow a number of the data elements listed above to be supported where not currently supported by the FHIR standard: 
  * UK Core extensions
    * The [UKCore-Evidence](https://simplifier.net/guide/uk-core-implementation-guide-stu2/Home/ProfilesandExtensions/ExtensionLibrary/Extension-UKCore-Evidence?version=2.0.1) extension provides a reference to results of investigations that confirmed the certainty of the diagnosis. Examples might include results of skin prick allergy tests.
* The `AllergyIntolerance.code` field **SHALL** be populated to identify the allergy or intolerance
* The `AllergyIntolerance.patient` field **SHALL** be populated.


|Name|ID Type|Unique ID|Description|Usage
|----|-------|---------|-----------|-----
HDUHBPASIdentifier|uri|https://fhir.hduhb.nhs.wales/Id/pas-identifier|This namespace indicates a Hywel Dda University Health Board PAS patient identifier|Patient identity
HDUHBPASIdentifier|oid|2.16.840.1.113883.2.1.8.1.3.149|This namespace indicates a Hywel Dda University Health Board PAS patient identifier|Patient identity
HDUHBPASPractitionerIdentifier|uri|https://fhir.hduhb.nhs.wales/Id/pas-practitioner-identifier|This namespace indicates a Hywel Dda University Health Board PAS practitioner identifier|Practitioner identity
PTHBPASAppointmentIdentifier|uri|https://fhir.pthb.nhs.wales/Id/pas-event-identifier|This namespace indicates a Powys Teaching Health Board PAS appointment identifier.|Appointment identity
PTHBPASIdentifier|uri|https://fhir.pthb.nhs.wales/Id/pas-identifier|This namespace indicates a Powys Teaching Health Board PAS patient identifier|Patient identity
PTHBPASIdentifier|oid|2.16.840.1.113883.2.1.8.1.3.170|This namespace indicates a Powys Teaching Health Board PAS patient identifier|Patient identity
PTHBPASPractitionerIdentifier|uri|https://fhir.pthb.nhs.wales/Id/pas-practitioner-identifier|This namespace indicates a Powys Teaching Health Board PAS practitioner identifier|Practitioner identity
SBUHBPASAppointmentIdentifier|uri|https://fhir.sbuhb.nhs.wales/Id/pas-event-identifier|This namespace indicates a Swansea Bay University Health Board PAS appointment identifier.|Appointment identity
SBUHBPASIdentifier|uri|https://fhir.sbuhb.nhs.wales/Id/pas-identifier|This namespace indicates a Swansea Bay University Health Board PAS patient identifier|Patient identity
SBUHBPASIdentifier|oid|2.16.840.1.113883.2.1.8.1.3.108|This namespace indicates a Swansea Bay University Health Board PAS patient identifier|Patient identity
SBUHBPASIdentifier|other|108|This namespace indicates a Swansea Bay University Health Board PAS patient identifier|Patient identity
SBUHBPASPractitionerIdentifier|uri|https://fhir.sbuhb.nhs.wales/Id/pas-practitioner-identifier|This namespace indicates a Swansea Bay University Health Board PAS practitioner identifier|Practitioner identity
VUNHSTCaniscIdentifier|uri|https://fhir.vunhst.nhs.wales/Id/canisc-identifier|This namespace indicates a Velindre University NHS Trust Canisc (PAS) patient identifier|Patient Identity
VUNHSTCaniscIdentifier|oid|2.16.840.1.113883.2.1.8.1.3.182|This namespace indicates a Velindre University NHS Trust Canisc (PAS) patient identifier|Patient Identity
VUNHSTCaniscIdentifier|other|182|This namespace indicates a Velindre University NHS Trust Canisc (PAS) patient identifier|Patient Identity
VUNHSTPASAppointmentIdentifier|uri|https://fhir.vunhst.nhs.wales/Id/pas-event-identifier|This namespace indicates a Velindre University NHS Trust PAS appointment identifier.|Appointment identity
VUNHSTPASPractitionerIdentifier|uri|https://fhir.vunhst.nhs.wales/Id/pas-practitioner-identifier|This namespace indicates a Velindre University NHS Trust PAS practitioner identifier|Practitioner Identity
CTMUHBPASIdentifier|uri|https://fhir.ctmuhb.nhs.wales/Id/pas-identifier|This namespace indicates a Cwm Taf Morgannwg University Health Board PAS patient identifier|Patient identity
CTMUHBPASIdentifier|oid|2.16.840.1.113883.2.1.8.1.3.126|This namespace indicates a Cwm Taf Morgannwg University Health Board PAS patient identifier|Patient identity
CTMUHBPASAppointmentIdentifier|uri|https://fhir.ctmuhb.nhs.wales/Id/pas-event-identifier|This namespace indicates a Cwm Taf Morgannwg University Health Board PAS appointment identifier.|Appointment identity
CAVUHBPASPractitionerIdentifier|uri|https://fhir.cavuhb.nhs.wales/Id/pas-practitioner-identifier|This namespace indicates a Cardiff and Vale University Health Board PAS practitioner identifier|Practitioner identity
CAVUHBPASAppointmentIdentifier|uri|https://fhir.cavuhb.nhs.wales/Id/pas-event-identifier|This namespace indicates a Cardiff and Vale University Health Board PAS appointment identifier.|Appointment identity
BCUHBPASPractitionerIdentifier|uri|https://fhir.bcuhb.nhs.wales/Id/pas-practitioner-identifier|This namespace indicates a Betsi Cadwaladr University Health Board PAS practitioner identifier. All BCUHB PAS instances have been consolidated into one system and the BCUHB namespace is now the primary identifier.|Practitioner identity
BCUHBPASAppointmentIdentifier|uri|https://fhir.bcuhb.nhs.wales/Id/pas-event-identifier|This namespace indicates a Betsi Cadwaladr University Health Board PAS appointment identifier. All BCUHB PAS instances have been consolidated into one system and the BCUHB namespace is now the primary identifier.|Appointment identity
ABUHBPASPractitionerIdentifier|uri|https://fhir.abuhb.nhs.wales/Id/pas-practitioner-identifier|This namespace indicates an Aneurin Bevan University Health Board PAS practitioner identifier|Practitioner identity
ABUHBPASPatientIdentifier|uri|https://fhir.abuhb.nhs.wales/Id/pas-identifier|This namespace indicates an Aneurin Bevan University Health Board PAS patient identifier|Patient identity
ABUHBPASPatientIdentifier|oid|2.16.840.1.113883.2.1.8.1.3.139|This namespace indicates an Aneurin Bevan University Health Board PAS patient identifier|Patient identity
TCLSpecimenTypeCodeIdentifier|uri|https://fhir.nhs.wales/Id/lims-tcl-specimen-type|This namespace is an identifier for a Trac Care Lab (LIMS) specimen type code|LIMS diagnostic specimen type code identifier
TCLReportCodeIdentifier|uri|https://fhir.nhs.wales/Id/lims-tcl-report-code|This namespace is an identifier for a Trac Care Lab (LIMS) report code|LIMS diagnostic report code identifier
TCLReportIdentifier|uri|https://fhir.nhs.wales/Id/lims-tcl-identifier|This namespace is an identifier for a Trac Care Lab (LIMS) report|LIMS diagnostic report
TCLReportIdentifier|oid|2.16.840.1.113883.2.1.8.1.3.154|This namespace is an identifier for a Trac Care Lab (LIMS) report|LIMS diagnostic report
TCLProcedureCodeIdentifier|uri|https://fhir.nhs.wales/Id/lims-tcl-procedure-code|This namespace is an identifier for a Trac Care Lab (LIMS) procedure code|LIMS diagnostic procedure code identifier
TCLeSpecimenTypeCodeIdentifier|uri|https://fhir.nhs.wales/Id/lims-tcle-specimen-type|This namespace is an identifier for a Trac Care Lab (LIMS2) specimen type code|LIMS2 diagnostic specimen type code identifier
TCLeReportCodeIdentifier|uri|https://fhir.nhs.wales/Id/lims-tcle-report-code|This namespace is an identifier for a Trac Care Lab (LIMS2) report code|LIMS2 diagnostic report code identifier
TCLeReportIdentifier|uri|https://fhir.nhs.wales/Id/lims-tcle-identifier|This namespace is an identifier for a Trac Care Lab (LIMS2) report|LIMS2 diagnostic report
TCLeReportIdentifier|oid|2.16.840.1.113883.2.1.8.1.3.328|This namespace is an identifier for a Trac Care Lab (LIMS2) report|LIMS2 diagnostic report
TCLeProcedureCodeIdentifier|uri|https://fhir.nhs.wales/Id/lims-tcle-procedure-code|This namespace is an identifier for a Trac Care Lab (LIMS2) procedure code|LIMS2 diagnostic procedure code identifier
WRTSLocationIdentifier|uri|https://fhir.nhs.wales/Id/wrts-location-identifier|N/A|Location Identifier
VUNHSTPASIdentifier|uri|https://fhir.vunhst.nhs.wales/Id/pas-identifier|This namespace indicates a Velindre University NHS Trust PAS patient identifier|Patient Identity
VUNHSTPASIdentifier|oid|2.16.840.1.113883.2.1.8.1.3.310|This namespace indicates a Velindre University NHS Trust PAS patient identifier|Patient Identity
VUNHSTPASIdentifier|other|131|This namespace indicates a Velindre University NHS Trust PAS patient identifier|Patient Identity
GPClusterCode|uri|https://fhir.nhs.wales/Id/gpcluster-code|This namespace indicates a Wales GP Cluster code|Organization identity
WRTSOrganizationIdentifier|uri|https://fhir.nhs.wales/Id/wrts-organization-identifier|N/A|Do not use
WRRSReportIdentifier|uri|https://fhir.nhs.wales/Id/wrrs-report-identifier|N/A|This namespace indicates an NHS Wales WRRS Report Id
WRRSMasterReportIdentifier|uri|https://fhir.nhs.wales/Id/wrrs-master-report-identifier|N/A|This namespace indicates an NHS Wales WRRS Master Report Id
DataStandardsWalesLIMSIdentifier|uri|https://fhir.nhs.wales/Id/lims-identifier|N/A|This namespace indicates an NHS Wales LIMS Identifier
HDUHBPASAppointmentIdentifier|uri|https://fhir.hduhb.nhs.wales/Id/pas-event-identifier|This namespace indicates a Hywel Dda University Health Board PAS appointment identifier.|Appointment identity
CTMUHBPASPractitionerIdentifier|uri|https://fhir.ctmuhb.nhs.wales/Id/pas-practitioner-identifier|This namespace indicates a Cwm Taf Morgannwg University Health Board PAS practitioner identifier|Practitioner identity
CAVUHBPASIdentifier|uri|https://fhir.cavuhb.nhs.wales/Id/pas-identifier|This namespace indicates a Cardiff and Vale University Health Board PAS patient identifier|Patient identity
CAVUHBPASIdentifier|oid|2.16.840.1.113883.2.1.8.1.3.140|This namespace indicates a Cardiff and Vale University Health Board PAS patient identifier|Patient identity
ApplicationInstanceIdentifier|uri|https://fhir.nhs.wales/Id/application-instance-identifier|This namespace indicates an NHS Wales Application Instance identifier|Patient identity
ApplicationInstanceIdentifier|oid|2.16.840.1.113883.2.1.8.1.5|This namespace indicates an NHS Wales Application Instance identifier|Patient identity
ABUHBPASAppointmentIdentifier|uri|https://fhir.abuhb.nhs.wales/Id/pas-event-identifier|This namespace indicates an Aneurin Bevan University Health Board PAS appointment identifier|Appointment identity
BCUHBPASIdentifier|uri|https://fhir.bcuhb.nhs.wales/Id/pas-identifier|This namespace indicates a Betsi Cadwaladr University Health Board PAS patient identifier. All BCUHB PAS instances have been consolidated into one system and the BCUHB namespace is now the primary identifier.|Patient identity
BCUHBPASIdentifier|oid|2.16.840.1.113883.2.1.8.1.3.109|This namespace indicates a Betsi Cadwaladr University Health Board PAS patient identifier. All BCUHB PAS instances have been consolidated into one system and the BCUHB namespace is now the primary identifier.|Patient identity
NADEXIdentifier|uri|https://fhir.nhs.wales/Id/nadex-identifier|This namespace indicates an NADEX identifier|Organization identity

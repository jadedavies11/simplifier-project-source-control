<div class="warning"><span class="ImplementWarn"></span></div>

## {{page-title}}

### Overview
The [Appointment](https://www.hl7.org/fhir/r4/Appointment.html) resource primarily allows the recording of detailed information about a planned meeting that may be in the future or past. The resource only describes a single meeting, a series of repeating visits would require multiple appointment resources to be created for each instance.

Examples include a scheduled surgery, a follow-up for a clinical visit, a scheduled conference call between clinicians to discuss a case, the reservation of a piece of diagnostic equipment for a particular use, etc. The visit scheduled by an appointment may be in person or remote (by phone, video conference, etc.) All that matters is that the time and usage of one or more individuals, locations and/or pieces of equipment is being fully or partially reserved for a designated period of time.

The {{page-title}} profile is derived from the [UK Core Appointment Profile](https://simplifier.net/guide/UK-Core-Implementation-Guide-STU2/Home/ProfilesandExtensions/Profile-UKCore-Appointment?version=2.0.1). It defines additional rules for use within health and care organisations in Wales.

A direct link to the Data Standards Wales asset can be accessed here - {{link:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Appointment}}

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Appointment, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Appointment, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-Appointment, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
       <li>{{pagelink:Home/FHIR-Assets/Profiles-and-Extensions/Profiles/Examples/Example-DataStandardsWales-Appointment-FollowUp.page.md, text:Follow Up Appointment}}</li>            
    </list>
  </div>    
</div>

### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Home/Introduction/Profile-Descriptions/Mandatory-and-Must-Support-Data-Elements.page.md,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.

### Each Appointment must have:
* A status
* One or more participants (typically a patient, clinician or service, and a location for the appointment)

### Each Appointment must support:
* Booking organization i.e. Health Board or GP Practice
  * Use the Appointment.extension:bookingOrganization to reference the organization
* An identifier
  * The Appointment.identifier field SHOULD include all available identifiers
  * Typical identifiers include the PAS visit or event id
  * Namespaces for such identifiers are maintained for each PAS system in Wales on the {{pagelink:Home/FHIR-Assets/Naming-Systems.page.md, text:Naming Systems}} page
* One or more specialty codes, including
  * A code from the [UKCorePracticeSettingCode](https://simplifier.net/guide/UK-Core-Implementation-Guide-STU2/Home/Terminology/AllValueSets/ValueSet-UKCore-PracticeSettingCode.page.md?version=current) code system (aligned with the Core Reference Data standard Treatment Function Code)
  * A local sub-specialty code. See the {{pagelink:Home/FHIR-Assets/Naming-Systems.page.md, text:Naming Systems}} for the relevant namespaces
* A reason for the appointment (if known)
* Reference to the Observation, Condition, Procedure, or ImmunizationRecommendation that is the reason for the appointment (if known)
* Start and end times for the appointment
* The referral (ServiceRequest) this appointment is based on


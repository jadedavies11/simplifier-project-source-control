<div class="warning"><span class="ExperiWarn"></span></div>

## {{page-title}}
The [ServiceRequest](https://www.hl7.org/fhir/r4/ServiceRequest.html) resource contains information of a request for a procedure or diagnostic or other service to be planned, proposed, or performed, as distinguished by the ServiceRequest.intent field value, with or on a patient.

The {{page-title}} profile is derived from the [UK Core Service Request Profile](https://simplifier.net/guide/uk-core-implementation-guide-stu2/Home/ProfilesandExtensions/Profile-UKCore-ServiceRequest?version=2.0.1) and is therefore listed as experimental. It defines additional rules for use within health and care organisations in Wales.

A direct link to the Data Standards Wales asset can be accessed here - {{link:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-ServiceRequest}}

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-ServiceRequest, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-ServiceRequest, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-ServiceRequest, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>{{pagelink:Example-DataStandardsWales-ServiceRequest-PathologyOrder, text:Example ServiceRequest}}</li>
    </list>
  </div>    
</div>

## Implementation Guidance
This profile aligns with the [UK Core Service Request Profile](https://simplifier.net/guide/uk-core-implementation-guide-stu2/Home/ProfilesandExtensions/Profile-UKCore-ServiceRequest?version=2.0.1).


### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Home/Introduction/Profile-Descriptions/Mandatory-and-Must-Support-Data-Elements.page.md,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.
 
**Each Service Request must have:**  (change these to be bullets similar to Patient page)
1. A status
  * status codes are defined by HL7
  * use 'active' for all current service requests
  * where a SR has been cancelled use 'revoked' where the reason for cancellation is unknown
1. An intent code indicating whether the request is a proposal, plan, or order
1. A code defining what is being requested
  * For WPAS referrals, use the sub-specialty code for the service being requested.
  * include the HB namespace (each one has their own list of codes)
1. A subject (i.e the patient)

**Each Service Request must support:**
1. An identifier 
  * The `ServiceRequest.identifier` field **SHOULD** contain all available identifiers. Typical identifiers include:
    * Relevant business identifiers for the request, e.g. pas-eventcode  
    * NB refer to namespaces for HB specific values
1. A category
1. A priority
1. A reference to one or more specimens
1. When request was authored
  * this is the effective date of the service request
1. The requester
1. The performer
  * at a min **SHOULD** be the performing organisation (i.e HB)

<br><br>


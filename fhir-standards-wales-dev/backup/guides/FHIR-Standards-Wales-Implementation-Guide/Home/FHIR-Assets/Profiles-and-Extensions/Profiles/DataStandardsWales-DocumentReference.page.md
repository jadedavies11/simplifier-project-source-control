<div class="warning"><span class="ExperiWarn"></span></div>

## {{page-title}}
The [DocumentReference](https://www.hl7.org/fhir/r4/documentreference.html) resource profile is used to index a document, clinical note, or other binary object to make them available to a healthcare system. A document is some sequence of bytes that is identifiable, establishes its own context (e.g., what subject, author, etc. can be displayed to the user), and has defined update management. The DocumentReference resource can be used with any document format that has a recognized mime type and that conforms to this definition.

The {{page-title}} profile is derived from the [HL7 R4 DocumentReference](https://www.hl7.org/fhir/r4/documentreference.html). It defines additional rules for use within health and care organisations in Wales.

A direct link to the Data Standards Wales asset can be accessed here - {{link:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-DocumentReference}}

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
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-DocumentReference, snapshot}}
    </div>
    <div id="tabdiff" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-DocumentReference, diff}}
  </div>
    <div id="tabhybrid" class="tabcontent">
      {{tree:https://fhir.nhs.wales/StructureDefinition/DataStandardsWales-DocumentReference, hybrid}}
  </div>
  <div id="tabeg" class="tabcontent">
    <list>
      <li>{{pagelink:Example-DataStandardsWales-DocumentReference-EncounterBased, text: Example Document Reference - Encounter-based}}</li>
      <li>{{pagelink:Example-DataStandardsWales-DocumentReference-EventBased, text: Example Document Reference - Event-based}}</li>     
      <li>{{pagelink:Example-DataStandardsWales-DocumentReference-NotEventBased, text: Example Document Reference - Not event-based}}</li> 
      <li>{{pagelink:Example-DataStandardsWales-DocumentReference-MisfiledNotEventBased, text: Example Document Reference - Misfiled (document not event-based)}}</li>              
    </list>
  </div>  
</div>

### Mandatory and Must Support Data Elements
Refer to the {{pagelink:Home/Introduction/Profile-Descriptions/Mandatory-and-Must-Support-Data-Elements.page.md,text: Mandatory and Must Support}} page for guidance on how these elements should be interpreted.
 
Each DocumentReference must have:
1. A status
1. A digital status
1. One or more attachments as *either* a base 64 binary *or* a URL. 

Each DocumentReference must support:
1. One or more identifiers
1. A document status
1. An error status (applicable if document is entered in error)
1. A type
1. One or more categories
1. A subject
1. A date
1. One or more authors
1. One or more attesters
1. A custodian
1. One or more security labels
1. A practice setting
1. A source system
1. A version
<br>

The `DocumentReference.status` field **SHALL** be populated with with one of the following values defined by the FHIR standard:
- current
- superseded
- entered-in-error
<br>

The `DocumentReference.extension.digitalStatus` field **SHALL** be populated with with one of the following values defined by the FHIR standard:
- born-digital-document
- scanned-paper-document
- unknown
<br>

### Extensions
The extensions listed below allow a number of the data elements listed above to be supported where not currently supported by the FHIR standard:
  * Data Standards Wales extensions
    * {{pagelink:Extension-DataStandardsWales-DocumentDigitalStatus}} supports the capture of a mandatory indication of whether the document was born digital or scanned.
    * {{pagelink:Extension-DataStandardsWales-SourceSystem}} supports the identification of the system which supplied the document details.
    * {{pagelink:Extension-DataStandardsWales-DocumentVersion}} supports the capture of a document version as defined in FHIR R5.
    * {{pagelink:Extension-DataStandardsWales-DocumentAttester}} supports the capture of attester details as defined in FHIR R5 via a complex extension.
    * {{pagelink:Extension-DataStandardsWales-DocumentErrorStatus}} supports the exchange of information about the validity of the document.
    * {{pagelink:Extension-DataStandardsWales-DocumentErrorAction}} supports the capture of the error workflow actions that led to the current error status.
    * {{pagelink:Extension-DataStandardsWales-DocumentAttribute}} supports the capture of additional document metadata via a complex extension.



   

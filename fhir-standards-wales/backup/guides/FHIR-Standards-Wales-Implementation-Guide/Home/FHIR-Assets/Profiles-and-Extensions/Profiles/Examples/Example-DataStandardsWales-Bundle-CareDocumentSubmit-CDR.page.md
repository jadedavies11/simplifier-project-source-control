<div class="warning"><span class="DevWarn"></span></div>

## Example Message Bundle - Care Document Submit (Minimal Required CDR Data)
This example provides comprehensive coverage of the data that should be completed, where available, when submitting a care document to the Care Data Repository.  The scenario is a record of a dermatology consultation conducted face-to-face with the patient on the ward as part of a dermatology clinic session. To simplify the bundle, the same consultant is referenced as author, attester and senior responsible clinician (attender).  In practice there could be multiple individual practitioners fulfilling this set of roles.  

To clarify use, the DocumentReference resource entry contains both `content.attachment.data` and `content.attachement.url`. In practice the bundle would content only one of these fields:
* If the bundle carries the actual PDF content prior to storage by the Care Document Service, use `content.attachment.data` to carry the PDF content as a base 64 binary.
* If the document is already in the applicable document store, use `content.attachment.url` to point to the document location.

The bundle does not cover external supersession identifier, as the construction of the `DocumentReference.identifier` element in this case has not been finalised at the time of publication.

<div class="tab-wrap">
  <ul class="tab-head">
    <li class="tablink" onclick="openCity(this,'tabtree')" data-target="tabtree">
      Overview
    </li>
    <li class="tablink" onclick="openCity(this,'tabtable')" data-target="tabtable">
      Table
    </li>
    <li class="tablink tab-active" onclick="openCity(this,'tabxml')" data-target="tabxml">
      XML
    </li>    
    <li class="tablink" onclick="openCity(this,'tabjson')" data-target="tabjson">
      JSON
    </li>    
    <li class="tablink" onclick="openCity(this,'tabnarrative')" data-target="tabnarrative">
      Narrative
    </li>
  </ul>
  <div class="tab-main">
    <div id="tabtree" class="tabcontent">
      {{tree:Example-DataStandardsWales-Bundle-CareDocumentSubmit-CDR}}
    </div>
    <div id="tabtable" class="tabcontent">
      {{table:Example-DataStandardsWales-Bundle-CareDocumentSubmit-CDR}}
    </div>       
    <div id="tabxml" class="tabcontent active">      
      {{xml:Example-DataStandardsWales-Bundle-CareDocumentSubmit-CDR}}
    </div>
    <div id="tabjson" class="tabcontent">
      {{json:Example-DataStandardsWales-Bundle-CareDocumentSubmit-CDR}}
    </div>
  </div>
</div>
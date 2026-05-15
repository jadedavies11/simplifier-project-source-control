# Care Document Versions

## How versioning works in WCRS
In the Welsh Care Records Service (WCRS), each new version of a document was represented as a separate record with its own unique `wcrsDocumentId`. These records were linked together only through a shared `wcrsSupersessionSetId`, which identified the **supersession set** to which all versions belonged. 
This way earlier versions of a record could be retrieved by locating the same suppersession set id. 

## How versioning works in FHIR
In FHIR all the versions of a document will be under the same DocumentReference resource.
All versions are expressed as history versions of the same FHIR resource, not as separate resources. 

* The FHIR resource ID remains constant accross all versions. 
* Each update creates a new `_history` version of that same resource.

<br>
{{render:Diagrams-Document-version-handling}}
<br>


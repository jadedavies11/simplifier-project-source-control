# Care Document Versions
Historically, the Welsh Care Records Service (WCRS) has served as the all-Wales repository for clinical documents.  This role is being phased out under a planned migration of care documents and functionality into the FHIR-based Care Data Repository.  The approaches taken to document version handing are different between WCRS and FHIR.  This section explains the differences, and the approach taken to minimise disruption for client applications.

## How versioning works in WCRS
In the Welsh Care Records Service (WCRS), each new version of a document was represented as a separate record with its own unique `DocumentId`. These records were linked together only through a shared `DocumentSupersessionSetId`, which identified the **supersession set** to which all versions belonged. A `SetSequenceNumber` on each document record clarified the order of document versions within the supersession set for easy identification of the latest, and to make explicit the save sequence order of prior versions. Some applications have needed to use and store and use their own identifiers and a business version to support local processing. These are known as external supersession identifiers and follow a common structure that uniquely identifies the issuing authority and the document. In summary:

* The `DocumentSupersessionSetId` remains constant across all versions.
* Each document version record has a unique `DocumentId` and a `SetSequenceNumber` to clarify the order of document versions.
* All document versions of a supersession set could be retrieved using the common `DocumentSupersessionSetId`.
* Local supersession set identifiers are supported via composite identifier `ExternalSupersessionId`, structured as [issuing authority]|[identifier].

## How versioning works in FHIR
In FHIR all the versions of a document will be under the same DocumentReference resource, which represents a supersession set. All versions are expressed as history versions of the same FHIR resource, not as separate resources. 

* The FHIR resource ID remains constant across all versions. 
* Each update creates a new `_history` version of that same resource.
* All document versions of a supersession set could be retrieved by querying the specific resource id for its history.

The differences are illustrated in the figure below:

<br>
{{render:Diagrams-Document-version-handling}}
<br>

## Minimising disruption during transition
For new FHIR-compliant applications submitting and retrieving care documents, the FHIR id and version history will fulfil the needs for retrieval and sequence identification. Many existing applications, however, are dependent up the current combination of identifiers as used in WCRS. This situation is expected to persist over a number of years. The following steps have been taken to support processing during the transition to a FHIR-based application landscape for care documents:
* The new Care Documents Service will continue to generate supersession set identifiers and document identifiers for submitted documents, following the pattern used by WCRS.
* The DataStandardsWales-DocumentReference profile has dedicated identifier slices (and associated naming systems) for `documentId`, `supersessionSetId` and `externalSupersessionSetId`.
* The `externalSupersessionSetId` slice uses a similar approach to the WCRS `ExternalSupersessionId`, but substitutes the pipe separator beween issuing authority and identifier with a tilde, because pipe is a reserved character for FHIR processing.
* SetSequenceNumber is supported by a meta tag with `.system` = "seqno".
* The business version to supplement the `externalSupersessionSetId` can be captured using extension `versionR5`.

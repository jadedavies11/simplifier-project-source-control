# Document Error Workflow
There are occasions where a document is considered to be invalid. Such documents cannot be deleted as they may have been seen and acted upon. For end applications there may be a need to display these documents differently and to restrict related processing. In these cases the document will be clearly marked with a status of "entered-in-error". The storage of data associated with the error worklow will depend upon the applicable error process as covered in the sub-sections below.  

## Misfiling workflow
Misfiling is a two step process followed when a user identifies that a document has been added to the wrong patient record. In the first step the user proposes that the document is misfiled. The second step is for a user to review and accept or reject the misfile proposal. 

_Guidance on the use of FHIR resources and elements to support the misfiling workflow and appropriate retrieval of affected documents will be provided at a future release._

## Revocation workflow
Revocation is a single step process to flag the document as revoked. A document can be revoked for a variety of reasons, such as that it is no longer valid. For example a “Do not attempt resuscitation” instruction may be actively revoked by the patient.

_Guidance on the use of FHIR resources and elements to support the revocation workflow and appropriate retrieval of affected documents will be provided at a future release._
<br />
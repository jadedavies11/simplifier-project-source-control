# Document Error Workflow
The DocumentReference resource provides explicit support for two distinct error workflows - misfiling and revocation. In both cases the documents cannot be removed from the patient record as they may have been seen and acted upon. For end applications there may be a need to display the documents differently and to restrict related processing.

## Misfiling workflow
Misfiling is a two step process followed when a user identifies that a document has been added to the wrong patient record. In the first step the user proposes that the document is misfiled. The second step is for a user to review and accept or reject the misfile proposal. The workflow and the recommended use of status and dedicated error-related elements at each stage are illustrated below.
<br />
{{render:Diagrams-Document-misfile-workflow}}
<br />

The following examples represent a document that is valid and the same document after it has been misfiled: 
* {{pagelink:Example-DataStandardsWales-DocumentReference-NotEventBased, text: Example Document Reference - Not event-based}}
* {{pagelink:Example-DataStandardsWales-DocumentReference-MisfiledNotEventBased, text: Example Document Reference - Misfiled (document not event-based)}}

## Revocation workflow
Revocation is a single step process to flag the document as revoked. A document can be revoked for a variety of reason, such as that it is no longer valid. For example a “Do not attempt resuscitation” instruction may be actively revoked by the patient. The use of status and dedicated error-related elements in the case of revocation is illustrated below.
<br />
{{render:Diagrams-Document-revocation-workflow}}
<br />
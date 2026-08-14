# Document Error Workflow
There are occasions where a document is judged to be invalid. Such documents cannot be deleted as they may have been seen and acted upon. For end applications there may be a need to display these documents differently and to restrict related processing. In these cases the current version of the document will be amended to provide the information required for end systems to recognise, mark and handle these documents appropriately.

The storage of status data and metadata associated with the error workflow will depend upon the applicable error process as covered in the sub-sections below.

## Misfiling workflow

Misfiling is a two-step process followed when a user identifies that a document has been added to the wrong patient record. In the first step the user requests that the document should be misfiled. The second step is for a user to review and accept or reject the misfile.

{{render:Diagrams-Document-misfile-workflow}}

The key metadata associated with misfiling are **who** (the user), **when** (the timestamp) and **why** (reason text at each step of the workflow). These details are stored in a {{pagelink:DataStandardsWales-Task,text:Task}} resource with a `code` of “review-document-misfile” and an `intent` of “proposal”.  The `code` and `intent` elements are fixed values throughout the misfile workflow.

**At Step 1** the new Task has a `status` of “requested “ and the other metadata are captured in the Task as follows:
- `focus` is the applicable DocumentReference
- `requester` is the user that requested the misfile
- `authoredOn` is the timestamp applicable to the misfile request submission
- `note` contains the free text misfile reason (with user and timestamp)

The current document version is untrustworthy at this stage, so it carries a new meta tag of “errorstatus” with the display value “Potentially misfiled”.  This tag can be used for marking of untrustworthy documents in accordance with applicable policy.

**At Step 2** a reviewer decides whether to accept or reject the misfile request.  In either case the task is updated as follows:
- `status` is set as “completed”
- `lastModified` is the timestamp applicable to the misfile review submission
- `owner` is the user that reviewed the misfile
- `output` is added with `type` “misfile-review-outcome”

In the case that the misfile is accepted
- the `output.value` is set to “accepted”
- an additional `note` instance contains the free text misfile accepted reason (with user and timestamp)
- the “errorstatus” meta tag on the DocumentReference is updated to a display value of “Misfiled”
- the `status` of the DocumentReference is updated to “entered-in-error”

In the case that the misfile is rejected
- the `output.value` is set to “rejected”
- an additional `note` instance contains the free text misfile rejected reason (with user and timestamp)
- the “errorstatus” meta tag is removed from the DocumentReference

The FHIR model changes resulting from the workflow steps are illustrated below:

{{render:Diagrams-Document-misfile-workflow-fhir}}

The associated Provenance records for the creation, update and deprecation of the DocumentReference and Task resources are for audit purposes only.

## Revocation
Revocation is a single step process to flag the document as revoked. A document can be revoked for a variety of reasons, such as that it is no longer valid. For example, a patient may wish to revoke a documented “Do not attempt resuscitation” instruction.

{{render:Diagrams-Document-revocation}}

In the case of revocation, there is no workflow to manage via a Task resource. The act of revocation results in an update of the DocumentReference `status` to “entered-in-error” and the population of the meta tag “errorstatus” with the display value “Revoked”.  In this case the who, when and why metadata are available in the related {{pagelink:DataStandardsWales-Provenance,text:Provenance}} record, which has an `activity` code of “deprecate” to indicate that the record has become invalid or untrustworthy. A free text reason for revocation can be stored in the `reason.text` element of the Provenance record. The use of Provenance for typical revocation use cases is illustrated in the figure below:

{{render:Diagrams-Document-revocation-fhir}}
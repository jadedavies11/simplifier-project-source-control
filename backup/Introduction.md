## Introduction

The Child Protection Information Sharing (CP-IS) initiative aims to share information between NHS clinicians and Local Authority social care practitioners relating to children with either Child Protection, Looked After or Unborn Child care plans. It is currently live in unscheduled care settings and the [HL7 V3 message specification](https://digital.nhs.uk/services/child-protection-information-sharing-project/cp-is-domain-message-specification) is available to view.  

Relevant data is uploaded to NHS Spine by a Local Authority system where it can be queried by NHS clinicians/practitioners. A response is returned to the practitioner showing any plans in existence for the specified NHS number and also the details of any device or person who has previously submitted a query against that NHS number. Further details of the [FHIR resources which constitute the query response](https://simplifier.net/guide/ChildProtection/Designoverview) are available.

### Current use cases

Examples of use cases in unscheduled care which currently provide the business context for this information exchange are:-

- A clinician treating a child submits a query to CP-IS to see if any child protection information exists.The querying clinician is a registered "smartcard" user.
- A clinician treating a child has a system query performed for him/her. The querying system is identified along with a default nominated person who is responsible for CP-IS queries.

Further details of [current use cases](https://digital.nhs.uk/services/child-protection-information-sharing-project/benefits-of-child-protection-information-sharing) can be viewed.

### Future use cases

It is planned to roll out CP-IS to scheduled care settings, for which the following are example use cases:-

- A clinician seeing a child/pregnant woman for scheduled care wishes to know if the child has a care plan without alerting the social worker, in order to provide contextual care for that person.
- A clinician wishes to be able to alert a social care practitioner, if a child/pregnant woman on a plan misses a scheduled appointment, so that the practitioner can take appropriate action. 



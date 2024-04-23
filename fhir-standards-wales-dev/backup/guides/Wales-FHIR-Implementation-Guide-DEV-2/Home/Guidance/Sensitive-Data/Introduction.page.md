## {{page-title}}
Sensitive records relate directly to tests and results that are considered as highly confidential in nature. In NHS Wales systems, sensitive records (e.g. test results, clinical documents) are flagged,  requiring the user to 'break glass' in order to view that record.

This page describes how the Data Standards Wales profiles can support flagging FHIR resources as having sensitive data via the information in the resource metadata tag.

This implementation guide references the following profiles for Diagnostic Data.
* {{pagelink:DataStandardsWales-DiagnosticReport}}
* {{pagelink:DataStandardsWales-Observation}}
* {{pagelink:DataStandardsWales-ServiceRequest}}

## Security Labels

A [security label](http://hl7.org/fhir/R4/security-labels.html){_target=blank} is a concept attached to a resource or bundle that provides specific security metadata about the information it is fixed. The intent of a security label is that the recipient of resources or bundles with security-tags is obligated to enforce the handling caveats of the tags and carry the security labels forward as appropriate.


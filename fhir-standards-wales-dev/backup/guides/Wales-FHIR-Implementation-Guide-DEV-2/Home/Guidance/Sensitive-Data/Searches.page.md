# {{page-title}}

It **SHOULD** be possible to limit search results based on their confidentiality by using the querystring **_tag={CodeSystem|Code}**. Some examples include:

## Sensitive/Restricted
A client interested in all sensitive Diagnostic reports by Patient and Code can use the following query:

```
GET [base]/DiagnosticReport?patient=[id]&code=[code]&_tag=http://terminology.hl7.org/CodeSystem/v3-Confidentiality|R
```
A client interested in all sensitive Observations by Patient and Code can use the following query:
```
GET [base]/Observation?patient=[id]&code=[code]&_tag=http://terminology.hl7.org/CodeSystem/v3-Confidentiality|R
```
A client interested in all sensitive ServiceRequests by Patient and Code can use the following query:
```
GET [base]/ServiceRequest?patient=[id]&code=[code]&_tag=http://terminology.hl7.org/CodeSystem/v3-Confidentiality|R
```

## Non-Sensitive/Not Restricted
A client requesting non-sensitive Diagnostic data can either, not include the Tag as per the example below:
```
GET [base]/[resource]?patient=[id]&code=[code]
```
or may decide to include the _tag with a confidentiality of N
```
GET [base]/[resource]?patient=[id]&code=[code]&_tag=http://terminology.hl7.org/CodeSystem/v3-Confidentiality|N
```

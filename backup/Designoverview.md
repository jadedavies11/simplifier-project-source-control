## Design overview

### FHIR Design for Child Protection Information Sharing

The Child Protection Information Sharing message exchange is based on the [FHIR RESTful framework](https://www.hl7.org/fhir/http.html) within which transactions are performed directly on the server resource using an HTTP request/response.   

The request to SPINE from a practitioner is made using a [named operation](https://simplifier.net/guide/ChildProtection/OperationDefinitionCPIS-GetBundle) with input parameters. The output parameter from the operation is a FHIR bundle of type 'searchset'.   

The diagram below shows the resources which would be returned in the bundle and the main references which link them together.

### Child Protection Information Sharing NHS Query Response bundle   

<br>
{{render:CPIS-DesignOptions-5}}






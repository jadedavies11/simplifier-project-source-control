## {{page-title}}

As defined in Version Management and Asset Status the type and impact of changes affect the category of release and version number.  
The content below summarises the types of change that may result from application of the Wales FHIR Development Process, along with potential impact and examples. 

|Change Type|Definition and Impact|Examples|
|-----------|---------------------|--------|
|Breaking|Changes that make previously valid implementations invalid or incompatible. 
Requires implementers to update systems; older data may fail validation|Removing or renaming an element.
Changing cardinality (e.g., from 0..* to 1..1). 
Altering data types in a way that existing data no longer conforms|
|Substantive|Significant changes that affect meaning or interpretation but do not necessarily break compatibility.
Implementers may need to review workflows or mappings, but existing data usually remains valid.|Adding new optional elements.
Changing descriptions or definitions that alter clinical meaning.|
|Non-Substantive (Editorial)|TCosmetic or clarifying changes that do not affect functionality or semantics.
Usually no effect on implementations but can become breaking if it invalidates a reasonable interpretation of the previously documented use of an element.|Fixing typos.
Improving documentation or examples.|
|Technical Corrections|Fixes to errors in the specification that were unintended. 
Usually minor but can become breaking where the change makes previously valid implementations invalid or incompatible|Correcting a wrong binding or constraint.|

Given the impact a breaking or non-compatible change may have on implementers, users of this Implementation Guide may find it useful to refer to the [HL7 FHIR Interversion Compatibility Page](https://confluence.hl7.org/spaces/FHIR/pages/35718683/Interversion+Compatibility) for a more comprehensive, but not exhaustive, list of breaking changes.
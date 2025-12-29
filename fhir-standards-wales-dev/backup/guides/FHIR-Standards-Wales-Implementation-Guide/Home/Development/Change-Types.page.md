## {{page-title}}

As defined in {{pagelink:Version-Policy-and-Format}} the type and impact of changes affect the category of release and version number.  
The content below summarises the types of change that may result from application of the Wales FHIR Development Process, along with potential impact and examples. 


<table class="table table-striped">
    <thead>
        <tr>
            <th scope="col">Change</th>
            <th scope="col">Definition and Impact</th>
            <th scope="col">Example</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td scope="row">Breaking</td>
            <td><p>Changes that make previously valid implementations invalid or incompatible.<p>
            <p>Requires implementers to update systems; older data may fail validation.<p></td>
            <td><p>Removing or renaming an element.<p>
            <p>Changing cardinality (e.g., from 0..* to 1..1).<p>
            <p>Altering data types in a way that existing data no longer conforms.<p></td>
        </tr>
        <tr>
            <td scope="row">Substantive</td>
            <td><p>Significant changes that affect meaning or interpretation but do not necessarily break compatibility.<p>
            <p>Implementers may need to review workflows or mappings, but existing data usually remains valid.<p></td>
            <td><p>Adding new optional elements.<p>
            <p>Changing descriptions or definitions that alter clinical meaning.<p></td>
        </tr>
        <tr>
            <td scope="row">Non-Substantive (Editorial)</td>
            <td><p>Cosmetic or clarifying changes that do not affect functionality or semantics.<p>
            <p>Usually no effect on implementations but can become breaking if it invalidates a reasonable interpretation of the previously documented use of an element.<p></td>
            <td><p>Fixing typos.<p>
            <p>Improving documentation or examples.<p></td>
        <tr>
            <td scope="row">Technical Corrections</td>
            <td><p>Fixes to errors in the specification that were unintended.<p>
            <p>Usually minor but can become breaking where the change makes previously valid implementations invalid or incompatible.<p></td>
            <td><p>Correcting a wrong binding or constraint.<p></td>
        </tr>    
    </tbody>
</table>

Given the impact a breaking or non-compatible change may have on implementers, users of this Implementation Guide may find it useful to refer to the [HL7 FHIR Interversion Compatibility Page](https://confluence.hl7.org/spaces/FHIR/pages/35718683/Interversion+Compatibility) for a more comprehensive, but not exhaustive, list of breaking changes.
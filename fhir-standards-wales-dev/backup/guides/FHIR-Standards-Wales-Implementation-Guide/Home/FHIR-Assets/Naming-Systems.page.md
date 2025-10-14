<div class="warning"><span class="ImplementWarn"></span></div>

# {{page-title}}
The following published Naming Systems are for use within Wales. 

## UK Wide Terminology Services

There are several namespaces used throughout this guide that are UK based which can be found on the [UK Naming Systems](https://simplifier.net/guide/uknamingsystems) page. These are not maintained by NHS Wales.


## OIDs

Data Standards Wales is responsible for the creation of namespaces and OIDs for NHS Wales systems. If you require one to be created please contact them using the email on the {{pagelink:Home/Help-and-Support/Help-and-Support.page.md,text:help and support}} page and ask for the link to the request form (internal to NHS Wales).

As there are several hundred systems currently registered with OIDs it has been decided that they will not all be added as naming systems. To be pragmatic, we have added the most used, high-level system identifiers shared between systems. Please remember that identifiers are extensible so you are not limited to only referencing the below namespaces. Further information can be found on the {{pagelink:Home/Design/Naming-Systems.page.md}} design page.

## List of Available Naming Systems

{{namingsystems}} 

<details>
    <summary>Section One</summary>
<br>
<table>
    <tr>
        <th>Name</th>
        <th>ID Type</th>
        <th>Unique ID</th>
        <th>Description</th>
        <th>Usage</th>
    </tr>
    <tr>
        <td>HDUHBPASIdentifier</td>
        <td>uri</td>
        <td>https://fhir.hduhb.nhs.wales/Id/pas-identifier</td>
        <td>This namespace indicates a Hywel Dda University Health Board PAS patient identifier</td>
        <td>Patient identity</td>
    </tr>
    <tr>
        <td>HDUHBPASIdentifier</td>
        <td>oid</td>
        <td>2.16.840.1.113883.2.1.8.1.3.149</td>
        <td>This namespace indicates a Hywel Dda University Health Board PAS patient identifier</td>
        <td>Patient identity</td>
    </tr>
    <tr>
        <td>HDUHBPASPractitionerIdentifier</td>
        <td>uri</td>
        <td>https://fhir.hduhb.nhs.wales/Id/pas-practitioner-identifier</td>
        <td>This namespace indicates a Hywel Dda University Health Board PAS practitioner identifier</td>
        <td>Practitioner identity
PTHBPASAppointmentIdentifier</td>
        <td>uri</td>
        <td>https://fhir.pthb.nhs.wales/Id/pas-event-identifier</td>
        <td>This namespace indicates a Powys Teaching Health Board PAS appointment identifier.</td>
        <td>Appointment identity</td>
    </tr>
    <tr>
        <td>PTHBPASIdentifier</td>
        <td>uri</td>
        <td>https://fhir.pthb.nhs.wales/Id/pas-identifier</td>
        <td>This namespace indicates a Powys Teaching Health Board PAS patient identifier</td>
        <td>Patient identity</td>
    </tr>
    <tr>
        <td>PTHBPASIdentifier</td>
        <td>oid</td>
        <td>2.16.840.1.113883.2.1.8.1.3.170</td>
        <td>This namespace indicates a Powys Teaching Health Board PAS patient identifier</td>
        <td>Patient identity</td>
</table>
</details>

<details>
    <summary>Section One</summary>
<br>
<table>
    <tr>
        <th>Name</th>
        <th>ID Type</th>
        <th>Unique ID</th>
        <th>Description</th>
        <th>Usage</th>
    </tr>
    <tr>
        <td>TCLSpecimenTypeCodeIdentifier</td>
        <td>uri</td>
        <td>https://fhir.nhs.wales/Id/lims-tcl-specimen-type</td>
        <td>This namespace is an identifier for a Trac Care Lab (LIMS) specimen type code</td>
        <td>LIMS diagnostic specimen type code identifier</td>
    </tr>
    <tr>
        <td>TCLReportCodeIdentifier</td>
        <td>uri</td>
        <td>https://fhir.nhs.wales/Id/lims-tcl-report-code</td>
        <td>This namespace is an identifier for a Trac Care Lab (LIMS) report code</td>
        <td>LIMS diagnostic report code identifier</td>
    </tr>
    <tr>
        <td>TCLReportIdentifier</td>
        <td>uri</td>
        <td>https://fhir.nhs.wales/Id/lims-tcl-identifier</td>
        <td>This namespace is an identifier for a Trac Care Lab (LIMS) report</td>
        <td>LIMS diagnostic report</td>
    </tr>
    <tr>
        <td>TCLReportIdentifier</td>
        <td>oid</td>
        <td>2.16.840.1.113883.2.1.8.1.3.154</td>
        <td>This namespace is an identifier for a Trac Care Lab (LIMS) report</td>
        <td>LIMS diagnostic report</td>
    </tr>
</table>
<details>
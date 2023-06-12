## Design Queries
Outstanding queries and issues relating to this specification are listed below:-   

- Can the following data items be retrieved from NHS Spine for the NHS Query using data supplied in the JSON Web Token by the client requestor   
    - effective time
    - organisation ODS or site code
    - organisation name
    - For a device as author
        - device identifier
    - For a person as author
        - Job role code
        - Job role name
        - SDS user ID
        - SDS role profile ID
        - Name details including prefix and suffix plus use value and validTime.start and end dates of the person's name?
- For both the NHS Query and the Query response, the person name.use element has different values in the HL7 V3 specification from the required values mandated in FHIR R4 for this element - these must be accurately mapped in a ConceptMap.
- Additional information has been inserted into the NHS Query response where the author is a device e.g. a distributed system such as the 111 service. This includes:-
    - The geographical/physical location of the patient which is inserted into the name element of the organisation which owns the device.
    -  The job role code, name and telephone number of the Safeguarding Lead at the geographical/physical location of the patient which is inserted into the Job role code element of the person assigned to the device.
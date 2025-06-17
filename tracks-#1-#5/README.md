# Tracks #1 and #5

Both tracks #1 and #5 will focus on maximizing the Terminology Servers by retrieving value set codes from the servers. Track #1 will utilize the FHIRLab FHIR server and track #5 will utilize the SEIR FHIR server.

The Immunization FHIR® Connectathon 2025 will use the **draft** [Immunization FHIR Implementation Guide](https://build.fhir.org/ig/UP-Manila-SILab/immunizationfhirig/index.html) with references pointing to the **draft** [PH Core FHIR Implementation Guide](https://build.fhir.org/ig/UP-Manila-SILab/ph-core/artifacts.html).

> [!CAUTION]
> **The Immunization FHIR IG and PH Core FHIR IG are made available for this track in initial draft forms with limited resources - The IGs are not suitable for production use or advanced testing.**

## FHIR Servers available for testing

Track | Version | Server | Endpoint
|----------|-------------|---------|-------------|
Track #1 | R4 | UPM SILab (FHIRLab) |https://cdr.fhirlab.net/fhir 
Track #5 | R4 | Pointwest (SEIR)    |https://hapifhir-api-128112993769.asia-southeast1.run.app

Note: FHIRLab is an open interoprability sandbox. FHIR server in FHIRLab will remain accessible for testing and on-going learning activites post connectathon.

## Additional tools provided for connectathon

The tools below allow you to perform experimentation immediately and interact with others. They are the preferred method of exploring FHIR at the connectathon.

- [Postman Collection](../sample-data) 
- [FHIR validator](https://validator.fhirlab.net)
- [Sample JSON files for PH Core profile](https://build.fhir.org/ig/UP-Manila-SILab/ph-core/artifacts.html#example-example-instances)

## Activity 1: Utilize the Terminology Server and Retrieve Value Set Codes

| Step | Activity                                       | Notes                                                                 | 
|------|------------------------------------------------|-----------------------------------------------------------------------|
| 1    | Review Immunization FHIR IG Value Sets         | Official URL of Value Sets were provided.                             |
| 2    | Setup access to test FHIR server               |                                                                       |
| 3    | Get `Vaccine Brand Name` Value Set             | $expand can be used to display Value Set codes.|
| 4    | Get `Vaccine Generic Name` Value Set           | $expand can be used to display Value Set codes.|
| 5    | Get `Action Taken` Value Set                    | $expand can be used to display Value Set codes.|
| 6    | Get `Action Reason` Value Set                   | $expand can be used to display Value Set codes.|
| 7    | Get `Vaccination Encounter Type` Value Set      | $expand can be used to display Value Set codes.|
| 8    | Get `Administrative Gender` Value Set           | This is a required Value Set in FHIR. $expand can be used to display Value Set codes.|


### Use Case Success
Server returns HTTP 200 OK with full Value Set response.

### Sequence Diagram
![alt text](<FHIR PH Immunization Sequence Diagram - UC1,5.png>)

### Acceptance Criteria
For a more detailed overview of the acceptance criteria of Use Cases (Tracks) #1 and #5, please refer to the [Acceptance Criteria Google Sheet UC#1,5](https://docs.google.com/spreadsheets/d/1OF5Jh_beGjB9nB7WSfQ_H10fC_Z-4T_4dBGndu6mgoQ/edit?gid=507922979#gid=507922979)

## Assumptions

Assumption | Details
|----------|-------------|
Non FHIR National Codes | For [Philippine Standard Geographic Code (PSGC)](https://psa.gov.ph/classification/psgc) and [National Health Facility Registry (NHFR)](https://nhfr.doh.gov.ph/VActivefacilitiesList), please refer to respective websites for more details on getting their standard codes.
Storage of Codes | It is recommended for this event for your application to store your copy of the PSGC and NHFR codes.
Facility Code | For this Connectathon, please assign your own organization a Facility Code that will be used throughout the event.

## Supplimentary guides for local testing

- [Starting a HAPI server - `FHIR CLI`](https://hapifhir.io/hapi-fhir/docs/tools/hapi_fhir_cli.html#server-run-server): Offers the endpoints above
- [Uploading FHIR IGs - `UploadFIG`](https://github.com/brianpos/UploadFIG#user-content-running-the-utility)
- [Uploading Resources - `Postman local app`](https://www.postman.com/downloads/)
- [Validating Resources - `FHIR validator`](https://confluence.hl7.org/spaces/FHIR/pages/35718580/Using+the+FHIR+Validator)




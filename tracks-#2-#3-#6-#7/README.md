# Tracks #2, #3, #6 and #7

Tracks #2, #3, #6, and #7 are all used for documenting the details of vaccine administration to patients. Tracks #2 and #6 are for submitting individual patient bundles while tracks #3 and #7 are for submitting bulk data.

The Immunization FHIR® Connectathon 2025 will use the **draft** [Immunization FHIR Implementation Guide](https://build.fhir.org/ig/UP-Manila-SILab/immunizationfhirig/index.html) with references pointing to the **draft** [PH Core FHIR Implementation Guide](https://build.fhir.org/ig/UP-Manila-SILab/ph-core/artifacts.html).

> [!CAUTION]
> **The Immunization FHIR IG and PH Core FHIR IG are made available for this track in initial draft forms with limited resources - The IGs are not suitable for production use or advanced testing.**

## FHIR Servers available for testing

Track | Version | Server | Endpoint
|----------|-------------|---------|-------------|
Track #2 and #3 | R4 | UPM SILab (FHIRLab) |https://cdr.fhirlab.net/fhir 
Track #6 and #7 | R4 | Pointwest (SEIR)    |https://hapifhir-api-128112993769.asia-southeast1.run.app

Note: FHIRLab is an open interoprability sandbox. FHIR server in FHIRLab will remain accessible for testing and on-going learning activites post connectathon.

## Additional tools provided for connectathon

The tools below allow you to perform experimentation immediately and interact with others. They are the preferred method of exploring FHIR at the connectathon.

- [Postman Collection](../postman-collection) 
- [FHIR validator](https://validator.fhirlab.net)

## Activity 2: Validate and submit a FHIR Bundle resource for an individual patient (Track 2 and 6)

| Step | Activity                                       | Notes                                                                 | 
|------|------------------------------------------------|-----------------------------------------------------------------------|
| 1    | Review Immunization FHIR IG Resources               | Refer to Resource Profiles found on the [Immunization FHIR IG Artifacts](https://build.fhir.org/ig/UP-Manila-SILab/immunizationfhirig/artifacts.html). |
| 2    | Setup access to test FHIR server                    | Refer to the environment under the [Postman Collection](../postman-collection) folder.  |
| 3    | Create a Resource `Bundle` for an individual patient| A bundle is a container for a collection of resources. Use provided examples.|
| 4    | `$validate` the Resource Bundle                     |                                                                       |
| 5    | Submit `Bundle` to FHIR Server                      |                                                                       |

### Use Case Success
- Created a Bundle for an individual patient
- IG validation is passed and server returns 200 OK
- Individual patient bundle posted to server and returns HTTP 200 OK
- Response status for each resource submitted is 201 Created

### Sequence Diagram
![alt text](<FHIR PH Immunization Sequence Diagram - UC 2,6.png>)

---

## Activity 3: Validate and submit a FHIR Bundle resource for multiple patients/bulk data (Track 3 and 7)
| Step | Activity                                       | Notes                                                                 | 
|------|------------------------------------------------|-----------------------------------------------------------------------|
| 1    | Review Immunization FHIR IG Resources               | Refer to the Resource Profiles found on the [Immunization FHIR IG Artifacts](https://build.fhir.org/ig/UP-Manila-SILab/immunizationfhirig/artifacts.html).|
| 2    | Setup access to test FHIR server                    | Refer to the environment under the [Postman Collection](../postman-collection) folder.|
| 3    | Create a Resource `Bundle` for multiple patients    | Create at least 5 individual patients in one resource bundle.         |
| 4    | `$validate` the Resource Bundle                     |                                                                       |
| 5    | Submit `Bundle` to FHIR Server                      |                                                                       |

### Use Case Success
- Created a Bundle for multiple patients
- IG validation is passed and server returns 200 OK
- Bulk data posted to server and returns HTTP 200 OK
- Response status for each resource submitted is 201 Created

### Sequence Diagram
![alt text](<FHIR PH Immunization Sequence Diagram - UC 3,7.png>)

## Acceptance Criteria

For a more detailed overview of the acceptance criteria of Use Cases (Tracks) #2, #3, #6 and #7, please refer to the [Acceptance Criteria Google Sheet UC#2,3,6,7](https://docs.google.com/spreadsheets/d/1OF5Jh_beGjB9nB7WSfQ_H10fC_Z-4T_4dBGndu6mgoQ/edit?gid=888992278#gid=888992278)

## Assumptions

Assumption | Details
|----------|-------------|
Non FHIR National Codes | For [Philippine Standard Geographic Code (PSGC)](https://psa.gov.ph/classification/psgc) and [National Health Facility Registry (NHFR)](https://nhfr.doh.gov.ph/VActivefacilitiesList), please refer to respective websites for more details on getting their standard codes.
Storage of Codes | It is recommended for this event for your application to store your copy of the PSGC and NHFR codes.
Facility Code | For this Connectathon, please assign your own organization a Facility Code that will be used throughout the event.

## Supplimentary guides for local testing

- [Starting a HAPI server - `FHIR CLI`](https://hapifhir.io/hapi-fhir/docs/tools/hapi_fhir_cli.html#server-run-server)
- [Uploading FHIR IGs - `UploadFIG`](https://github.com/brianpos/UploadFIG#user-content-running-the-utility)
- [Uploading Resources - `Postman local app`](https://www.postman.com/downloads/)
- [Validating Resources - `FHIR validator`](https://confluence.hl7.org/spaces/FHIR/pages/35718580/Using+the+FHIR+Validator)


# Use Case #1 and #5

The Immunization FHIR® Connectathon 2025 will use the **draft** [Immunization FHIR Implementation Guide](https://build.fhir.org/ig/UP-Manila-SILab/immunizationfhirig/index.html) with references pointing to the **draft** [PH Core FHIR Implementation Guide](https://build.fhir.org/ig/UP-Manila-SILab/ph-core/artifacts.html).

> [!CAUTION]
> **The Immunization FHIR IG and PH Core FHIR IG are made available for this track in initial draft forms with limited resources - The IGs are not suitable for production use or advanced testing.**

## FHIR Servers available for testing

FHIR Server | Version | UPM SILab (FHIRLab) | Pointwest (SEIR)
|----------|-------------|---------|-------------|
Use Case #1 and #5 | R4 | https://cdr.fhirlab.net/fhir |https://hapifhir-api-128112993769.asia-southeast1.run.app

Note: FHIRLab is an open interoprability sandbox. FHIR server in FHIRLab will remain accessible for testing and on-going learning activites post connectathon.

## Additional tools provided for connectathon

The tools below allow you to perform experimentation immediately and interact with others. They are the preferred method of exploring FHIR at the connectathon.

- [Postman Collection with example requests] **Insert link here** (../sample-data/fhir_resources_collection.json)
- [FHIR validator](https://validator.fhirlab.net)
- [Sample JSON files for PH Core profile](https://build.fhir.org/ig/UP-Manila-SILab/ph-core/artifacts.html#example-example-instances)

## Assumptions

Assumption | Details
|----------|-------------|
Non FHIR National Codes | For [Philippine Standard Geographic Code (PSGC)](https://psa.gov.ph/classification/psgc) and [National Health Facility Registry (NHFR)](https://nhfr.doh.gov.ph/VActivefacilitiesList), please refer to respective websites for more details on getting their standard codes.
Storage of Codes | It is recommended for this event for your application to store your copy of the PSGC and NHFR codes.
Facility Code | For this Connectathon, please assign your own organization a Facility Code that will be used throughout the event.

## Track success 

1. Submit FHIR resource to $validate against FHIR IG
2. Server returns Operation Outcome with success or conformance errors (fix errors and validate again)
3. IG validation is passed
4. Create individual resources such as, Patient → Encounter → Condition → Medication → Observation
5. Server returns HTTP 201 Created
6. Create and Send resources in one Bundle
7. Server processes and returns HTTP 200 with full Bundle response

## Aceeptance Criteria

For the Acceptance Criteria of Use Cases #1 and #5, please refer to the [Acceptance Criteria Google Sheet UC#1,5](https://docs.google.com/spreadsheets/d/1OF5Jh_beGjB9nB7WSfQ_H10fC_Z-4T_4dBGndu6mgoQ/edit?gid=507922979#gid=507922979)


## Supplimentary guides for local testing

- [Starting a HAPI server - `FHIR CLI`](https://hapifhir.io/hapi-fhir/docs/tools/hapi_fhir_cli.html#server-run-server): Offers the endpoints above
- [Uploading FHIR IGs - `UploadFIG`](https://github.com/brianpos/UploadFIG#user-content-running-the-utility)
- [Uploading Resources - `Postman local app`](https://www.postman.com/downloads/)
- [Validating Resources - `FHIR validator`](https://confluence.hl7.org/spaces/FHIR/pages/35718580/Using+the+FHIR+Validator)




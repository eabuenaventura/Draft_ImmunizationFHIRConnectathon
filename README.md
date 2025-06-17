 # Immunization FHIR® Connectathon – June 2025, Tagaytay City, Philippines

![alt text](<Immunization Connectathon Graphic.png>)

The 2025 Immunization FHIR® Connectathon is hosted and co-organized by the Standards and Interoperability Laboratory (UPM SILab), under the University of the Philippines Manila National Institutes of Health’s National Telehealth Center (NTHC) together with the Department of Health (DOH) and United Nations Children's Fund (UNICEF). This program is supported by the Australian Government Department of Foreign Affairs and Trade (DFAT) with technical assistance from the Commonwealth Scientific and Industrial Research Organisation (CSIRO). 

The Immunization Connectathon is part of UP Manila's Long-Term Agreement with UNICEF with its first engagement focusing on Interoperability Development and Implementation: Implementing a standards-based immunization Implementation Guide through the use of international terminology and data exchange standards.

The project's objectives are as follows:
- Develop the necessary interoperability resources to ensure linkage of SEIR with other systems. **(FHIR® Immunization Implementation Guide)**
- Develop a sandbox environment for testing and capacity building. **(FHIR® Test Environment)**
- Engage, capacitate, and support the EMR providers/developers and other system owners in adopting interoperability standards and connecting to SEIR. **(Immunization Connectathon)**

## Important Information

- [Immunization Connectathon Program (June 18 to 20, 2025)](https://docs.google.com/document/d/1ZhGiq2hBP_GjHPMt0mrmMDQac4xZioBsp2v8EPYcqfU/edit?usp=drive_link)
- [Immunization Connectathon Logistic Note](https://docs.google.com/document/d/1fbSN0oHLXzEBDl8HvAIGGM-8iRUYSdeACN44viK4x20/edit?usp=drive_link) 

## Immunization Connectathon Objectives 

| Objective | Details | 
|-----------------|-----------------|
| Data Exchange      | Successfully exchange immunization records using FHIR Immunization resource with at least two other participants (to SEIR and from another participant) |
| Terminology Mapping  | Validate use of existing codes across the test scenarios |
| Profile Conformance  | Validate conformance to the draft Immunization Implementation Guide with the draft PH Core IG as reference |
| Client-Server Interactions  | Demonstrate read, search, and update interactions between client apps and FHIR servers|
| Record Validation  | Cross-check vaccination records for completeness based on the Immunization Minimum Data Set |
| Feedback and Reporting  | Submit structured feedback on gaps in profile conformance, terminology, or server responses |
  
## Use Case Summary (Tracks)

| **HAPI FHIR:** FHIR Lab | **HAPI FHIR:** Pointwest HAPI FHIR| 
|-----------------|-----------------|
| 1. Users will maximize Terminology Server. **(GET)** | 5. Users will maximize Terminology Server. **(GET)** |
| 2. Users will submit INDIVIDUAL data. **(POST)** | 6. Users will submit INDIVIDUAL data. **(POST)** |
| 3. Users will submit BULK data. **(POST)** | 7. Users will submit BULK data. **(POST)** |
| 4. Users will retrieve vaccine record. **(GET)**  | 8. Users will retrieve vaccine record. **(GET)** |

## Tracks and Sample Data

- [Tracks #1 and #5](tracks-%231-%235)
- [Tracks #2, #3, #6, and #7](tracks-%232-%233-%236-%237)
- [Tracks #4 and #8](tracks-%234-%238)
- [Postman Collection and Environment](postman-collection)


---

Note: FHIR® is a registered trademark of Health Level Seven International.  

For questions and queries regarding connectathon, contact silab.upm@up.edu.ph

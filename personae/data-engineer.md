# Persona: Paul Garcia

| Age | 35  |
| --- | --- |
| Occupation | Data Engineer |
| Specialization | Data infrastructure and management in healthcare |
| Experience | 10 years in healthcare IT, focusing on research data solutions |
| Location | CHUV, Switzerland |
| Analytics Proficiency | Expert in database management, cloud computing, APIs, and healthcare data standards |
| CHORUS Role | Data Admin |

## User Story: Make available patient cohort exploration data (HORUS explorer) to researchers

As Paul García, Data Engineer, **I want to** automatically deploy and easily configure a custom service/application **so that I** can load requested patient data with predefined scripts. The requestors will be automatically notified once the data is delivered in prod.

## Goals

- Streamline data access for researchers by providing self-service tools for patient cohort exploration.
- Automate routine tasks related to cohort data exploration, ensuring researchers can find relevant data without needing constant IT support. Automate data provisioning on a regular basis (daily basis).
- Ensure efficient communication with data requestor using the required ticketing system

## Frustrations

- Need to do manual and repetitive tasks daily that could be automated.
- Data is not available in clinical data warehouse or needs to be transformed (cleansing and standardization), incurring additional complex tasks
- Data specification is not clearly defined
- Requests coming from different communication channels
- Cannot communicate directly with data requestor

## Requirements

| Legal | Follow legal requirements (authorization to transfer data – DTA, DTUA) |
| --- | --- |
| Data | Pseudo-coded data according to legal requirements (if we don’t have SPARC, do we deliver anonymized data?) |
| Infrastructure | Database location can be in the local CHUV clinical network or in CHORUS (cloud)<br><br>Data Admin role defined in CHORUS<br><br>Ticketing system and standard request forms |
| Software and tools | Access to interfaces to deploy apps and load data |
| Support | Access to CHORUS support team<br><br>Access to documentation |

## Scenario

| CHUV Ticketing system (outside CHORUS) | Paul receives a request for service deployment (HORUS explorer) and data loading with all required specifications (ideally provided in a standard form) |
| --- | --- |
| CI/CD, workflow | He automatically deploys the service into CHORUS prod |
| Project Workspace | Paul checks the availability of the service (frontend, backend, databases check), and sets up the authentication (provide valid CHUV user access to app requestor, if no CHUV active directory - how to manage users?) |
| Outside CHORUS | Paul needs to verify the availability of required specifications and complete them if necessary (contact requestor): Requestor workspace (data destination), Inclusion/exclusion criteria (patient cohort definition), variables for research, ethical (research protocol) requirements, legal requirements (CHUV DTA) |
| CHUV Ticketing system (outside CHORUS) | He forwards requests to a data analyst if they are specific (variables requiring additional data collection) |
| Data Engineer workstation | Paul prepares the data release and loads into the test environment |
| Project Workspace | Paul validates the delivery in the prod environment by running test queries |
| CHUV Ticketing system (outside CHORUS) | He closes the ticket, and the requestor is notified automatically |
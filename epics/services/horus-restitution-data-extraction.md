# Horus Restitution - Data Extraction

## Goal
To extract de-identified data from the Clinical Research Data Warehouse (DWH-C) for a clinical study in a CHORUS workspace

## User Stories

### Clinical Researcher Story

**Persona:**
Dr. Marie Fischer, Chief Resident and Clinical Researcher in the Department of Oncology (@personae/principal-investigator.md)

**As** a Clinical Researcher
**I want to** securely extract de-identified patient data for my approved study
**So that** I can conduct my clinical research with the necessary data while ensuring patient privacy

**Acceptance Criteria:**
1. Can access CHORUS with CHUV credentials
2. Can navigate to project workspace
3. Can submit a data extraction request through the standardized form
4. Can provide all necessary documentation (ethics approval, study protocol)
5. Can track the status of my request through Jira
6. Can receive notifications about request updates
7. Can access the extracted data in my CHORUS workspace
8. Can verify the completeness and quality of received data

**Steps:**
1. Access the CHUV research portal (CHORUS) and log in with CHUV account
2. Navigate to project workspace
3. Follow the getting started guide to understand the data extraction process
4. Submit a data restitution request via the form:
   https://jira.chuv.ch/servicedesk/customer/portal/1/create/30
5. Provide all required information and documentation in the ticket
6. Receive confirmation and track progress through Jira
7. Access data in the CHORUS workspace once processed

### Data Engineer Story

**Persona:**
Paul García, Data Engineer (@personae/data-engineer.md)

**As** a Data Engineer
**I want to** process and fulfill data extraction requests efficiently and securely
**So that** researchers can receive their required data while maintaining compliance with all regulations and requirements

**Acceptance Criteria:**
1. Can receive and review data extraction requests
2. Can verify all required specifications and documentation
3. Can communicate with requestors for additional information
4. Can validate data extraction criteria
5. Can prepare and test data in a staging environment
6. Can ensure proper de-identification of data
7. Can deliver data to the correct workspace
8. Can maintain audit trail of the entire process

**Steps:**
1. Receive and review data extraction request with specifications from researcher
2. Verify completeness of request including:
   - Requestor workspace (data destination)
   - Inclusion/exclusion criteria (patient cohort definition)
   - Variables for research
   - Ethical requirements (research protocol)
   - Legal requirements (CHUV DTA)
3. Forward specific requests to data analysts if needed
4. Prepare and validate data in test environment
5. Verify data quality and de-identification in production
6. Deploy data to researcher's workspace
7. Close ticket with appropriate documentation 
# Horus Explorer - Feasibility Study

## Goal
To determine the number of existing patients in the Clinical Research Data Warehouse (DWH-C) for a clinical study

## User Stories

### Clinical Researcher Story

**Personas:**
- Dr. Marie Fischer, Chief Resident and Clinical Researcher in the Department of Oncology (@personae/principal-investigator.md)
- Dr David Ortega, Clinical Researcher (@personae/hip-researcher.md)

**As** a Clinical Researcher
**I want to** quickly determine the number of eligible patients for my study
**So that** I can assess the feasibility of my clinical study before committing resources

**Acceptance Criteria:**
1. Can log in to CHORUS with CHUV credentials
2. Can access Horus Explorer with proper authorization
3. Can define patient inclusion/exclusion criteria
4. Can execute feasibility queries
5. Can view the number of eligible patients
6. Can export feasibility results
7. Can save queries for future reference

**Steps:**
1. Access the CHUV research portal (CHORUS) and log in with CHUV account
2. Learn about the procedures for creating a clinical study through available documentation
3. Follow the getting started guide to perform a feasibility query
4. Request access to Horus Explorer via CHUV form:
   https://formulaire.chuv.ch/sites/acces/Horus/Lists/Demandes/NewForm.aspx?Source=https%3A%2F%2Fformulaire%2Echuv%2Ech%2Fsites%2Facces%2FHorus%2FSitePages%2FAccueil%2Easpx&RootFolder=
5. Receive confirmation of Active Directory access enablement via email
6. Log in to Horus Explorer and perform feasibility query
7. Analyze results to determine study feasibility

### Data Engineer Story

**Persona:**
Paul García, Data Engineer (@personae/data-engineer.md)

**As** a Data Engineer
**I want to** efficiently process and manage access requests for Horus Explorer
**So that** researchers can quickly determine the feasibility of their studies while maintaining system security

**Acceptance Criteria:**
1. Can receive access requests through the standardized system
2. Can verify requester credentials and permissions
3. Can process access requests in a timely manner
4. Can maintain security audit logs
5. Can revoke access when needed

**Steps:**
1. Receive access request from researcher
2. Validate the request and user credentials
3. Grant appropriate access levels
4. Notify researcher of access approval

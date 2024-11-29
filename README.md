# CHORUS Platform Requirements

## Overview
This repository contains the requirements for the CHORUS (CHUV Research Platform) platform, which facilitates clinical research by providing secure access to clinical data while ensuring compliance with privacy regulations and research protocols.

## Repository Structure

```
.
├── epics/                      # Epic-level documentation
│   ├── template-epic.md       # Template for creating new epics
│   └── services/              # Services-related epics
│       ├── README.md          # Services overview
│       ├── horus-explorer.md  # Feasibility study service
│       ├── horus-restitution-data-extraction.md  # Data extraction service
│       └── horus-restitution-admin.md  # Data administration service
└── personae/                  # User personas documentation
    ├── principal-investigator.md
    ├── hip-researcher.md
    └── data-engineer.md
```

## Documentation Structure

### Epics
Each epic follows a standardized structure:
- Vision and Goals
- Business Value
- Success Metrics (KPIs)
- Dependencies
- Constraints
- User Stories with Acceptance Criteria

### Services
The platform currently provides the following core services:
1. **Horus Explorer** - Feasibility studies for clinical research
2. **Horus Restitution - Data Extraction** - Secure data extraction for approved studies
3. **Horus Restitution - Data Administration** - Data quality management and annotation
4. **Horus Dataset Catalog** - (Coming soon)

### User Personas
Documentation includes detailed user personas representing key stakeholders:
- Principal Investigators
- Clinical Researchers
- Data Engineers
- Data Managers

## Contributing
When contributing to this documentation:
1. Use the provided epic template (`epics/template-epic.md`)
2. Follow the established structure for consistency
3. Include clear acceptance criteria and steps
4. Reference appropriate user personas

## Related Resources
- [CHUV Research Portal](https://research.chuv.ch)
- [Horus Explorer Access](https://formulaire.chuv.ch/sites/acces/Horus)
- [Data Request Form](https://jira.chuv.ch/servicedesk/customer/portal/1/create/30) 
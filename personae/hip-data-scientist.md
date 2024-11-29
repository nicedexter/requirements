# Persona: Jonathan Dan

| Age | 32  |
| --- | --- |
| Occupation | Biomedical Engineer |
| Specialization | Signal processing, epilepsy |
| Experience | Postdoctoral researcher, medical sensors, wearable EEG, signal processing, machine learning |
| Location | EPFL, Switzerland |
| Analytics Proficiency | Python, PyTorch, Docker containers |
| CHORUS Role | Workspace Member |

## User Story: Launch and manage a research project on CHORUS

As Jonathan Dan, a Postdoctoral Researcher in the Embedded Systems Laboratory at EPFL, **I want to** design and provide a standardized and well-documented framework for evaluating EEG-based seizure detection algorithms **so that I can** share it with the machine learning community and enable to compare algorithm performances in a reliable and reproducible way, ultimately contributing valuable findings to the epilepsy research community.

## Goals

- Develop a unified framework (Seizure score: SzCORE) to standardize the validation of EEG-based seizure detection algorithms, improving consistency and comparability across studies.
- Set a clear standard for algorithm evaluation (introduce the 10-20 seizure detection benchmark, a machine-learning benchmark based on public datasets converted to a standardized format)
- Make the SzCORE framework and benchmark publicly accessible to facilitate rigorous, clinically significant evaluation of seizure detection algorithms.
- Make validated algorithms available through the platform.

## Frustrations

- Heterogeneity in EEG data formats and content
- Heterogeneity in validation methods—such as different datasets, evaluation methods, and metrics—makes it difficult to comprehensively evaluate and compare algorithms.
- Varying performance metrics used in current research hinder clear comparison and understanding of algorithm effectiveness.
- Limited access to standardized datasets and lack of open resources impedes collaborative efforts in the field, slowing progress toward optimized seizure detection.

## Requirements

| Data | Access/import public data to use for testing. This data can be viewed by all users within the workspace. |
| --- | --- |
|     | Send algorithm for testing on clinical study/private data set and only communicate back anonymized statistical result(s). I do not access/view the data. |
| Able to handle following data:<br><br>Type: Scalp-EEG<br><br>Format: edf (raw EEG data); tsv (seizure annotations); json (metadata)<br><br>Size: 1 TB |
| Algorithms | Have the possibility to keep algorithms private. |
| Import algorithms as Docker containers (not as apps, not needing to “re-initiate” HIP) |
| Update SzCORE website automatically with testing results. |
| Software | Python, PyTorch |

## Scenario

| Homepage Overview | Marie navigates to the CHORUS website where she is presented with a clear and concise overview of CHORUS, including its purpose, features, and ongoing projects. |
| --- | --- |
| Homepage Access | She signs in to access her home dashboard for general information and her personal workspace for experimenting with data and analytical tools. |
| Project Lifecycle | Marie can access an overview of the project lifecycle describing the different steps, tasks and contacts relevant to her project giving her a clear view on how to best proceed. |
| Support and Documentation | She accesses comprehensive documentation, including research guidelines and best practices, data usage guidelines, tutorials, and contact information for support. |
| Dataset Exploration | Marie browses and searches through the available datasets, using filters based on inclusion criteria to determine whether she can use available data for her project. |
| Dataset Overview | She views detailed information about each dataset, including metadata, methodology, and associated publications. |
| Dataset Access | Marie requests access to specific datasets in a standardized format for further analysis. She is notified when she is granted access. |
| Data de-identification | She requests support for data de-identification to be able to share data with her external colleague. |
| Project Workspace | She requests creating a project workspace and is notified once it is active. She defines project members and their access rights (for internal and external collaborators). |
| Research/Analytics | Marie won’t be performing analysis. She has defined the scientific goals together with her colleague, AI professor (described in protocol). Three project members will perform data analysis accordingly. They will use Python with libraries xxx, 3D Slicer and FreeSurfer going through the App Store. |
| Results and publications | Marie can view and discuss the results within the project workspace. She can export graphics and tables to include in her presentations, reports and publications. |
| Collaborative Opportunities | The platform provides information on collaborative projects, and Marie can find opportunities to connect with other researchers working on related topics. |
| Feedback and Contribution | Marie provides feedback on the platform and contributes her own datasets and findings to enhance the resource for the scientific community. |
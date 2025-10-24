# Analysis of 2025 Health Insurance Exchange Public Use Files
The Centers for Medicare & Medicaid Services (CMS) Center for Consumer Information and Insurance Oversight (CCIIO) is committed to increasing transparency in the Health Insurance Exchanges. CMS publishes downloadable public use files (PUFs) so that researchers and other stakeholders can more easily access Exchange data.

## Table of Contents
- [Project Overview](#project-overview)
- [Data & Tools](#data-and-tools)
- [Dashboard Link](#dashboard-link)
- [Full Report](#full-report)
- [Data Preparation](#data-preparation)

## Project Overview
This analysis evaluates key indicators of health insurance market performance across the United States in 2025, focusing on premium costs, plan diversity, and issuer competitiveness. The dataset was sourced from the CMS Health Insurance Marketplace public use files, including plan attributes, benefits and cost sharing, network, issuer details and quality ratings for 2025. The analysis covers participating states and insurance issuers.

## Data and Tools
* Data Source: [CMS Health Insurance Marketplace Public Use Files (PUFs)](https://www.cms.gov/marketplace/resources/data/public-use-files)
* Tools: Tableau, Python (for cleaning), Excel (for cleaning)
* Visualization PlatformL Tableau Cloud
* Report Format: PDF Report + Interactive Tableau Dashboard

## Dashboard Link
[View Tableau Workbook File](./tableau%20dashboard)

## Full Report
[Read the Full Analytical Report (PDF)](https://ebanksdev.com/resume/Analysis%20of%202025%20Health%20Insurance%20Exchange%20Public%20Use%20Files.pdf)

## Data Preparation
Data was split using a python a script and preprocessed using python before cleaning inn excel and visualization in Tableau.

Key steps:
* Replaced null rows utilizing the data dictionary provided for context
* Checked for duplicates
* Ensured proper formatting and data consistency
* Created calculated fields and did QA checks
* Exported final dataset as `.csv for Tableau

  Below is a snapshot of part of the cleaning workflow
  Python Cleaning Script:<img width="909" height="366" alt="python script" src="https://github.com/user-attachments/assets/030ae6ba-be90-4785-9603-633a34da99e7" />

  An example of excel issues log: <img width="1850" height="574" alt="excel issues log" src="https://github.com/user-attachments/assets/3f06db0a-b89a-4107-917d-c141ae01b04e" />

Screenshot of Dashboard <img width="1373" height="896" alt="image" src="https://github.com/user-attachments/assets/41cbed79-70d7-40eb-b3b2-7558abf43eb6" />


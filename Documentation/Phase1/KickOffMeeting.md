# Project Charter: Patient Data Analysis

## Why is this analysis needed?
This analysis is needed to identify trends in patient admissions, diagnoses, hospital resource utilization, and financial costs. The insights will help optimize hospital operations.

## What business questions do stakeholders want answered through this analysis?
- What are the most common diagnoses and procedures?
- How does patient demographic data (age, gender, race, ethnicity) impact hospital visits?
- What are the trends in hospital stay duration and costs?
- Are there seasonal patterns in patient admissions?
- How can we improve resource allocation based on patient data?
- How do different admission types correlate with severity and patient outcomes?
- What factors contribute to readmission rates and patient mortality?

## Are there any Key Performance Indicators (KPIs) to measure?
- **Average Length of Stay (ALOS)** (based on `length_of_stay` column)
- **Readmission Rates** (based on `patient_disposition` and `discharge_year` columns)
- **Patient Mortality Rates** (`apr_risk_of_mortality`)
- **Cost per Patient Visit** (`total_charges` vs. `total_costs`)
- **Bed Occupancy Rate** (inferred from `facility_id` and `hospital_county`)
- **Percentage of High-Risk Patients** (`apr_severity_of_illness_description` and `apr_medical_surgical_description`)

## Is this the only dataset, or do we need to combine it with others?
Currently, the analysis is based on the provided `patients.csv` dataset, which includes patient demographics, hospital details, admission details, and financials. Additional datasets (e.g., billing records, patient feedback, electronic health records) may be required for deeper insights which will be included in future agile framework.

## Who owns the data (IT, Business, Finance, etc.)?
- **Primary Owner:** IT & Clinical Data Management Team
- **Contributors:** Business Intelligence, Research Team, Finance Department, Clinical Staff
- **Regulatory Oversight:** Compliance & Legal Teams (for HIPAA and data security)

## What format is preferred for final outputs (dashboard, report, presentation)?
- **Interactive Dashboard** Tableau showing KPIs, trends, and insights.
- **PDF Reports** with key findings for executive summaries.
- **Executive Presentation** PowerPoint summarizing actionable recommendations.

## Should the analysis be one-time or ongoing (quarterly, monthly, yearly)?
The analysis will be one time for now, as the business expand the ongoing analysis will be provided if needed.

## Are there any data access restrictions (e.g., HIPAA compliance for patient data)?
- Yes, patient data is subject to **HIPAA compliance** and must be handled securely.
- Personal Identifiable Information (PII) (e.g., `attending_provider_license_number`, `operating_provider_license_number`) must be anonymized before analysis.

## What’s the project deadline?
- **Initial findings & report:** 02/15/2025
- **Full dashboard implementation:** 02/25/2025
- **Ongoing analysis & improvements:** Bi-Weekly Updates

## When are progress updates expected?
- **Weekly team check-ins** to discuss progress & roadblocks.
- **Bi-weekly stakeholder updates** via email or presentations.
- **Monthly report submissions** for review.

## Are there any dependencies (e.g., waiting for more data)?
- Additional data sources may be required for in-depth analysis, but it's out of scope right now. 
- Compliance team must approve data handling procedures before sharing insights.
- Data cleaning and transformation steps must be completed before dashboard implementation.

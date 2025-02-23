# Project Charter: Patient Data Analysis

## 1. Why is this analysis needed?
This analysis is needed to identify trends in patient admissions, diagnoses, hospital resource utilization, and financial costs. The insights will help improve patient care, optimize hospital operations, and enhance financial decision-making.

## 2. What business questions do stakeholders want answered?
- What are the most common diagnoses and procedures?
- How does patient demographic data (age, gender, race, ethnicity) impact hospital visits?
- What are the trends in hospital stay duration and costs?
- Are there seasonal patterns in patient admissions?
- How can we improve resource allocation based on patient data?
- How do different admission types correlate with severity and patient outcomes?
- What factors contribute to readmission rates and patient mortality?

## 3. Are there any KPIs (Key Performance Indicators) to measure?
- **Average Length of Stay (ALOS)** (based on `length_of_stay` column)
- **Readmission Rates** (based on `patient_disposition` and `discharge_year` columns)
- **Patient Mortality Rates** (`apr_risk_of_mortality`)
- **Cost per Patient Visit** (`total_charges` vs. `total_costs`)
- **Bed Occupancy Rate** (inferred from `facility_id` and `hospital_county`)
- **Percentage of High-Risk Patients** (`apr_severity_of_illness_description` and `apr_medical_surgical_description`)

## 4. Is this the only dataset, or do we need to combine it with others?
Currently, the analysis is based on the provided `patients.csv` dataset, which includes patient demographics, hospital details, admission details, and financials. Additional datasets (e.g., billing records, patient feedback, electronic health records) may be required for deeper insights.

## 5. Who owns the data (IT, Business, Finance, etc.)?
- **Primary Owner:** IT & Clinical Data Management Team
- **Contributors:** Business Intelligence, Research Team, Finance Department
- **Regulatory Oversight:** Compliance & Legal Teams (for HIPAA and data security)

## 6. What format is preferred for final outputs (dashboard, report, presentation)?
- **Interactive Dashboard** (Power BI, Tableau) showing KPIs, trends, and insights.
- **PDF Reports** with key findings for executive summaries.
- **Executive Presentation** (PowerPoint) summarizing actionable recommendations.
- **Raw Data Summaries** for advanced analysis by research teams.

## 7. Should the analysis be one-time or ongoing (monthly, quarterly)?
The analysis should be **ongoing**, with reports generated on a **monthly** basis for trend monitoring and operational decision-making. Additionally, ad-hoc deep dives may be needed for specific inquiries.

## 8. Are there any data access restrictions (e.g., HIPAA compliance for patient data)?
- Yes, patient data is subject to **HIPAA compliance** and must be handled securely.
- Data access is restricted to authorized personnel only.
- Personal Identifiable Information (PII) (e.g., `attending_provider_license_number`, `operating_provider_license_number`) must be anonymized before analysis.
- Financial data (`total_charges`, `total_costs`) must be protected from unauthorized access.

## 9. What’s the project deadline?
- **Initial findings & report:** [Insert Date]
- **Full dashboard implementation:** [Insert Date]
- **Ongoing analysis & improvements:** Monthly Updates

## 10. When are progress updates expected?
- **Weekly team check-ins** to discuss progress & roadblocks.
- **Bi-weekly stakeholder updates** via email or presentations.
- **Monthly report submissions** for review.

## 11. Are there any dependencies (e.g., waiting for more data)?
- Additional data sources may be required for in-depth analysis.
- IT needs to validate data integrity before full analysis.
- Compliance team must approve data handling procedures before sharing insights.
- Data cleaning and transformation steps must be completed before dashboard implementation.

---
This document will be updated as new requirements emerge and feedback is received from stakeholders.

# Healthcare Analytics Dashboard

An interactive Power BI dashboard that analyzes hospital admissions, patient demographics, and billing revenue. It helps explore how patient volume and revenue vary across medical conditions, insurance providers, hospitals, and doctors over time.

## Dataset

The dataset contains 55,500 patient admission records with 15 columns, covering admissions from 2019 to 2024.

| Column | Description |
|---|---|
| Name | Patient name |
| Age | Patient age |
| Gender | Male / Female |
| Blood Type | Patient blood group |
| Medical Condition | Diagnosed condition (Arthritis, Diabetes, Hypertension, Obesity, Cancer, Asthma) |
| Date of Admission | Admission date |
| Doctor | Attending doctor |
| Hospital | Admitting hospital |
| Insurance Provider | Insurance company (Aetna, Blue Cross, Cigna, Medicare, UnitedHealthcare) |
| Billing Amount | Total billed amount |
| Room Number | Assigned room |
| Admission Type | Elective / Urgent / Emergency |
| Discharge Date | Discharge date |
| Medication | Prescribed medication |
| Test Results | Normal / Abnormal / Inconclusive |

## Data Preparation (Power Query)

- Standardized text casing in the Name column
- Removed duplicate records
- Converted admission and discharge columns to Date type
- Handled invalid (negative) billing amounts
- Cleaned the Hospital column and rounded Billing Amount to 2 decimals

## Dashboard Overview

The report has two pages with navigation buttons and shared slicers for Doctor, Hospital, Insurance Provider, and Date of Admission.

**Key metrics:** Total Revenue, Total Number of Admissions, Total Number of Hospitals, Total Number of Doctors

**Overview page**
- Patients by Blood Type, Medical Condition, Insurance Provider, and Medication
- Patients by Year (trend)
- Gender Distribution, Admission Type, Test Results, and Age Group breakdowns

**Revenue Information page**
- Revenue by Insurance Provider
- Revenue by Top 10 Hospitals
- Revenue by Admission Year
- Revenue by Top 10 Doctors

## Project Files

- `healthcare_dataset.csv` - Source dataset
- `images/overview_page.png` - Overview page screenshot
- `images/revenue_page.png` - Revenue Information page screenshot

## Dashboard Preview

### Overview
![Overview Page](Project Files/overview_page.png)

### Revenue Information
![Revenue Page](Project Files/revenue_page.png)

## Tools Used

- Power BI Desktop
- Power Query
- DAX

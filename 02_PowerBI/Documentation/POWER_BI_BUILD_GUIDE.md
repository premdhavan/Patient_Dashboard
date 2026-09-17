# Power BI Build Guide

## Important
A real `.pbix` file is a binary Power BI Desktop artifact and cannot be generated reliably in this Python environment. This repository therefore contains the complete GitHub-ready dataset, visual assets, DAX measures, Power Query reference, and a build guide. Open Power BI Desktop and build/save the final `.pbix` using these assets.

## Recommended report pages

### Page 1 — Patient Overview
**KPI cards**
- Total Patients
- Total Doctors
- Average Age
- Insurance Providers

**Visuals**
1. Clustered column: Patient Count by City
2. Bar: Patient Count by Chronic Condition
3. Line: Patient Count by Registration Year
4. Donut: Patient Count by Gender
5. Column: Patient Count by Age Group

**Slicers**
- Gender
- Age Group
- City
- Blood Group
- Marital Status
- Smoking Status
- Alcohol Consumption
- Chronic Condition
- Insurance Provider
- Registration Year

### Page 2 — Patient Details
Add a table/matrix containing:
Patient_ID, Gender, Age, Age Group, Blood_Group, Marital_Status, City, State,
Height_cm, Weight_kg, BMI, Smoking_Status, Alcohol_Consumption,
Chronic_Condition, Primary_Doctor_ID, Insurance_Provider, Registration_Date.

Use the slicers to demonstrate filtered results.

### Page 3 — Data Quality / Analysis
Suggested cards and visuals:
- Average BMI
- Patients with chronic condition
- Patients by smoking status
- Patients by alcohol consumption
- Patients by insurance provider
- Patients by doctor

## Data model
For this single-table project, a star schema is not required. Use the cleaned table as the main fact-like table. If you later add dimensions, create relationships using stable keys.

## Import
1. Open Power BI Desktop.
2. Get Data → Text/CSV.
3. Select `01_Dataset/Cleaned_Data/Patient_Cleaned_Data.csv`.
4. Load/Transform Data.
5. Confirm date fields are Date type and numeric fields are numeric.
6. Add the DAX measures from `04_DAX_Measures/Patient_Dashboard_Measures.dax`.
7. Add visuals and slicers according to the layout above.
8. Save as `Patient_Dashboard.pbix` in `02_PowerBI/`.
9. For GitHub, consider keeping only the `.pbix` if its size is suitable; otherwise publish the report separately and keep this repository as the project documentation/data package.

## Filtering demonstration
Use `City = Pune` as the example filter to reproduce the supplied filtered-data preview. The example CSV is already generated from the cleaned dataset.

## Privacy
The public-ready CSVs remove direct personal/contact fields from the supplied workbook. Do not upload the original workbook if it contains real patient or contact information.

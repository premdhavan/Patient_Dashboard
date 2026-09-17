# Patient Report Dashboard — Excel to Power BI

A GitHub-ready data analytics project based on the supplied **Patient Dashboard.xlsx** workbook. The project converts the Excel analysis into a Power BI-ready structure with raw/cleaned/filtered datasets, KPI definitions, visual references, DAX measures, Power Query guidance, and documentation.

## Project summary

The dataset contains **20,000 patient records**. The Excel workbook already included a raw patient master table, a cleaned table with an `Age Group` field, KPI calculations, chart summaries, and a dashboard layout.

### Key KPIs
| KPI | Value |
|---|---:|
| Total Patients | 20,000 |
| Total Doctors | 11 |
| Average Age | 43.88 |
| Insurance Providers | 5 |

## Dashboard visuals

The Power BI report is designed to include:
- KPI cards
- Patient count by city
- Patient count by chronic condition
- Patient count by registration year
- Patient count by gender
- Patient count by age group
- Patient detail table
- Interactive slicers
- Filtered-data demonstration

## Slicers / filters
Recommended slicers:
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

## Folder structure

```text
Patient_Dashboard_PowerBI_GitHub/
├── 01_Dataset/
│   ├── Raw_Data/
│   │   └── Patient_Raw_Data_Anonymized.csv
│   ├── Cleaned_Data/
│   │   └── Patient_Cleaned_Data.csv
│   ├── Filtered_Data/
│   │   └── Patient_Filtered_Pune_Example.csv
│   └── README.md
├── 02_PowerBI/
│   └── Documentation/
│       └── POWER_BI_BUILD_GUIDE.md
├── 03_Dashboard_Images/
│   ├── KPIs/
│   ├── Charts/
│   ├── Dataset_Previews/
│   └── dashboard_layout_preview.png
├── 04_DAX_Measures/
│   └── Patient_Dashboard_Measures.dax
├── 05_Power_Query/
│   └── Patient_Cleaned_Data_M_Query.txt
├── 06_Project_Documentation/
│   └── PROJECT_NOTES.md
├── 07_Excel_Dashboard/
│   └── Patient_Dashboard.xlsx
├── 08_PowerBI_Dashboard/
│   └── Patient Dashboard.pbix
└── README.md
```

## Data preparation

The original Excel workbook contained both raw and cleaned patient tables. The cleaned table adds `Age Group` for easier dashboard segmentation. The Power BI version should use the cleaned dataset as the primary table.

## Privacy note

The supplied workbook contains direct personal/contact-style fields such as names, phone numbers, email addresses, addresses and insurance policy numbers. For this GitHub package, those fields have been removed from the public-ready CSVs. **Do not upload the original workbook if the records are real.**

## Power BI file

A binary `.pbix` cannot be generated reliably outside Power BI Desktop. The repository therefore includes everything needed to create the report: datasets, dashboard preview images, DAX, Power Query guidance, and a step-by-step Power BI build guide.

After creating the report in Power BI Desktop, save it as:

`02_PowerBI/Patient_Dashboard.pbix`

## Tools

- Microsoft Excel
- Microsoft Power BI Desktop
- Power Query
- DAX
- CSV
- GitHub

## Project objective

Demonstrate an end-to-end analytics workflow:
**Raw Data → Cleaning → KPI Creation → Visualization → Interactive Filtering → Power BI Dashboard**


## Excel Dashboard Screenshot
<img width="1600" height="518" alt="Patient DashB SS" src="https://github.com/user-attachments/assets/8550881b-f1a9-4fef-845a-af417ca03322" />

## PowerBI Dashboard Screenshot
<img width="1138" height="644" alt="Patient PowerBI DashB SS" src="https://github.com/user-attachments/assets/c50ff99e-d9d5-41ed-8e29-9bd742f60405" />



## Author

**Prem Dhavan**
Data Analyst / BI Project Portfolio
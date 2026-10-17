# Hospital Operations & Patient Analytics | Power BI Project

A Power BI healthcare analytics project focused on hospital operations, patient admissions, department and doctor performance, waiting times, patient outcomes, revenue, profitability, and management KPIs.

This project brings multiple healthcare performance indicators into a five-page interactive dashboard to support operational monitoring and data-driven decision-making.

## Project Overview

The **Hospital Operations & Patient Analytics Dashboard** analyzes hospital visit records and supporting dimension tables to explore how patient activity, operational efficiency, clinical outcomes, and financial performance can be monitored in one reporting environment.

The dashboard is built using Microsoft Power BI and an Excel-based synthetic portfolio dataset. It combines patient and admission analysis with department performance, waiting-time monitoring, revenue analysis, and target comparisons.

### Project Objectives

- Monitor hospital visits and unique patient activity.
- Analyze patient demographics, visit types, admission patterns, and insurance categories.
- Compare department and doctor performance using visits, revenue, and profit.
- Examine waiting times, length of stay, readmission, and patient outcomes.
- Track revenue, treatment costs, profit, and reported target achievement.
- Identify data-quality and KPI-definition issues that should be validated before business use.

## Dashboard Pages

### 1. Hospital Executive Overview

Provides a high-level view of hospital activity and performance.

Key dashboard elements:
- Total visits and unique patients
- Total revenue and total profit
- Average waiting time and recovery rate
- Monthly patient visits and hospital revenue
- Visits by department and admission type
- Patient outcomes and hospital comparisons

### 2. Patient & Admission Analysis

Explores patient characteristics and healthcare utilization patterns.

Key dashboard elements:
- Patient and visit counts
- Visits by gender and age group
- Visit type and admission type distributions
- Insurance-type analysis
- New, returning, and referral patient categories
- Average length of stay and revenue per patient

### 3. Department & Doctor Performance

Compares department activity and reported financial contribution.

Key dashboard elements:
- Top 10 doctors by revenue
- Patient visits by department
- Revenue by department
- Doctor revenue compared with visit volume
- Department profit margin
- Department performance table with visits, revenue, profit, and revenue per visit

### 4. Operations & Waiting Time

Focuses on operational indicators and patient outcomes.

Key dashboard elements:
- Average waiting time
- Average length of stay
- Emergency visits
- Readmission rate and recovery rate
- Waiting time by department and admission type
- Monthly visits compared with average waiting time
- Patient outcomes by department

### 5. Revenue & Management

Focuses on financial performance and target monitoring.

Key dashboard elements:
- Total revenue and treatment cost
- Total profit and profit margin
- Revenue target and revenue growth
- Department revenue compared with target
- Monthly visits compared with visit targets
- Revenue by hospital and insurance type
- Profit by department and department target-performance indicators

## Dataset & Excel Workbook

The project uses a **synthetic portfolio dataset** supplied in an Excel workbook. The workbook contains the following sheets:

| Worksheet | Records, excluding header | Purpose |
|---|---:|---|
| `FactVisits` | 20,000 | Hospital visit and operational records |
| `DimPatient` | 5,000 | Patient attributes |
| `DimDoctor` | 105 | Doctor and specialization attributes |
| `DimDepartment` | 15 | Department information |
| `DimHospital` | 5 | Hospital information |
| `DimDate` | 730 | Calendar and date attributes |
| `Targets` | 360 | Target records |
| `Project_Info` | 1 | Project metadata |

The visit fact table supports analysis of admission and visit types, waiting time, length of stay, treatment costs, revenue, payment information, and patient outcomes.

The dimension sheets provide supporting patient, doctor, department, hospital, and date information. The `Targets` sheet supports target-oriented reporting.

> **Dataset note:** This is a synthetic portfolio project, not a report of actual hospital performance or real patient outcomes.

## Key Performance Indicators

The following figures are displayed in the supplied dashboard PDF. They are reported dashboard values and should not be interpreted as independently audited results.

| KPI | Reported value |
|---|---:|
| Total Visits | 20K |
| Unique Patients | 5K |
| Total Revenue | 140.34M |
| Total Profit | 48.61M |
| Average Waiting Time | 46.16 |
| Recovery Rate | 48.34% |
| Average Length of Stay | 1.33 |
| Readmission Rate | 2.99% |
| Total Treatment Cost | 91.74M |
| Profit Margin | 34.63% |
| Revenue Target | 120.03M |
| Revenue YoY Growth | 1,126.16% |

The unit and calculation definition of each KPI should be documented in the Power BI model. In particular, waiting time and length of stay should have clearly stated units.

## Analytical Observations

The dashboard is designed to help users investigate:

- Which departments and hospitals contribute the most visits and revenue.
- How patient volume varies by admission type, visit type, demographics, and insurance.
- How reported revenue and profit differ across departments.
- Where waiting times and length of stay vary between departments or admission categories.
- How reported hospital and department results compare with targets.
- Whether patient outcome categories and readmission measures are consistently defined.

These are analysis areas supported by the dashboard design. Specific performance conclusions should be drawn only after validating the underlying calculations and filters.

## Data Validation & Limitations

A review of the dashboard and workbook identified several items that should be checked before using the reported figures for decision-making:

1. **Date relationship and time intelligence:** Confirm that the fact-table date key matches the date dimension's relationship key. Validate the date relationship before relying on monthly trends or year-over-year calculations.
2. **Revenue YoY growth:** The dashboard displays 1,126.16% growth. This requires validation against the intended comparison period, date filters, and DAX measure.
3. **Different totals across visuals:** Some department-level totals differ from the executive-page totals. Check filter context, category coverage, and aggregation logic before treating these as directly comparable.
4. **Unique patient count:** Confirm that the KPI counts distinct patients represented in visit records rather than all records in the patient dimension.
5. **Target definitions:** Document whether targets are monthly, annual, department-level, or hospital-level, and verify that actuals and targets use comparable periods and filters.
6. **Outcome and operational measures:** Define the denominator and inclusion rules for recovery rate, readmission rate, average waiting time, and length of stay.

The dashboard figures are preserved as displayed in the supplied report. These validation notes identify checks to complete; they do not imply that the measures have already been corrected.

## Tools & Technologies

- **Microsoft Power BI Desktop** — dashboard development and interactive reporting
- **Microsoft Excel** — source workbook and dataset
- **Power Query** — data preparation and transformation, where used
- **DAX** — KPI calculations and measures, where implemented
- **Data modeling** — fact and dimension tables for analytical reporting

## Skills Demonstrated

- Healthcare operations analytics
- Patient and admission analysis
- Department and doctor performance analysis
- KPI reporting and dashboard design
- Revenue, cost, and profitability analysis
- Target monitoring
- Data modeling and metric validation
- Data visualization and business reporting

## Repository Structure

```text
Hospital-Operations-Patient-Analytics-Power-BI/
├── README.md
├── Hospital Operations Analysis.pbix
├── Hospital Operations Analysis.xlsx
└── screenshots/
    ├── hospital-executive-overview.png
    ├── patient-admission-analysis.png
    ├── department-doctor-performance.png
    ├── operations-waiting-time.png
    └── revenue-management.png
```

The screenshot filenames above are the proposed names for the five PDF pages. Add the corresponding PNG files before publishing the repository so the screenshot links can be verified.

## How to Explore the Project

1. Download or clone the repository.
2. Open the `.pbix` file using Microsoft Power BI Desktop.
3. Review the dashboard pages and available slicers.
4. Inspect the Excel workbook to understand the source tables.
5. Validate the data model, measures, date relationships, and target definitions before relying on the reported KPIs.

## Potential Applications

The analytical approach demonstrated in this portfolio project could support hospital management reporting, operational performance reviews, patient-flow monitoring, departmental comparisons, and financial KPI tracking. The synthetic dataset is intended for demonstration and learning, not clinical or operational decision-making.

## Author

**Altamash Nizamuddin**  
Data Analyst | Excel • Power BI • Python • MySQL

- GitHub: [@altamash-analyst](https://github.com/altamash-analyst)
- Email: [altamash9876@gmail.com](mailto:altamash9876@gmail.com)

## Repository Description

Power BI hospital operations dashboard analyzing patient visits, admissions, department and doctor performance, waiting times, patient outcomes, revenue, profit, and management targets using a synthetic Excel dataset.

## Suggested GitHub Topics

`power-bi` `hospital-analytics` `healthcare-analytics` `hospital-operations` `patient-analytics` `healthcare-dashboard` `business-intelligence` `data-analytics` `dax` `microsoft-excel` `operational-efficiency` `financial-analytics` `Altamash-Analyst`

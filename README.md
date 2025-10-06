# Healthcare-Data-Analysis
### Analysis of UK healthcare using Excel and Power BI

### Data Source
Kaggle open source data- [http//:Kaggle.com](https://www.kaggle.com/datasets)

### Data Governance 
All data used within this project/dashboard are entirely fictitious and generated for demonstration purposes. No real patient, staff, or organisational data are included. The dataset has been fully anonymised and does not contain any information that could directly or indirectly identify any real individual.

### Tools
- Excel- used for data Cleaning
- Powerbi for developing semantic models to implement interactive dashboards.

## Project Methodology & Data Analysis Summary

This section details the steps taken for data preparation, modeling, and visualization to generate actionable insights from the raw healthcare dataset.
1. Data Preparation and Cleaning (Microsoft Excel).
The raw data was initially processed and cleaned using Microsoft Excel to ensure high data quality and consistency across all tables.
Appointment	Table :
> Converted Appointment Date from whole numbers to the correct Date format using the Text-to-Columns feature.
> Data Type Transformation, Data Parsing : Doctors	Consolidated First Name and Last Name into a single, dedicated Doctor Name column.	
> Data Manipulation, Feature Engineering : Removed redundant columns (Email Address, Phone Number) to streamline the data model and improve query performance.
>Data Redundancy Reduction Patient Table:	Calculated the accurate age of each patient using the DATEDIF function against their date of birth.	
- Custom Column Calculation, Temporal Data Analysis
- Formatted the Registration column to display only the month and year for cohort analysis.	
> Data Formatting, Time Series Preparation
- Removed personally identifiable information (PII) like Email Address and Address.	Data Privacy & Simplification

### Data Modeling and Business Intelligence (Power BI)

Post-cleaning:
The Tables were  imported into Power BI to construct a robust, semantic data model, leading to the creation of the final interactive dashboard.

Relationship Mapping: Established a star schema by defining clear, logical relationships between the core data tables (e.g., Doctors, Patients, Appointments, and Bill). This ensures accurate filtering and aggregation across the dashboard.

Semantic Data Model Development: Created calculated measures and defined hierarchies within Power BI to support complex business questions and metrics (e.g., calculating Doctor Success Rate, Revenue Lost, and Appointment Distribution).

### Visualization and Dashboarding: Designed and developed a comprehensive dashboard to visualize key performance indicators (KPIs) and trends, including:
Appointment Status Distribution (Cancellation, No-Show Rates)
Financial Performance (Expected vs. Actual Revenue)
Top Performing Doctors and Specialties
Payer Mix and High-Cost Insurance Providers
<img width="1855" height="870" alt="Screenshot 2025-10-06 231006" src="https://github.com/user-attachments/assets/cdd2944a-06f4-47a6-81be-e3d7d0ecc0aa" />


### Key Dashboard Insights

## Patient and Appointment Overview: 
Small, Highly Engaged Patient Base: The clinic has 50 unique patients, and remarkably, 48 of them (96%) have had more than one visit. This suggests that while the patient volume is small, the clinic excels at getting patients to return.
High Specialist Demand: The clinic is heavily focused on Paediatrics (98 appointments) and Dermatology (70 appointments), which together account for the vast majority of appointments by specialty. This indicates these are the primary drivers of clinical activity.
Top 5 Doctor Concentration: The top five doctors handle a significant portion of the bookings (89 total), suggesting a high reliance on a few key practitioners.

> Critical Efficiency Issue: The allocation of appointment statuses raises significant concerns:
o Scheduled:
o Cancelled:
o No-Show:
• Analysis: About two-thirds (around 66%) of all appointments that were scheduled are NOT fulfilled because of cancellations or no-shows. This results in a substantial loss of time, income, and clinical resources

### Financial Performance: Notable Revenue Decline and Payer Composition
> The clinic faces a severe financial crisis, with Actual Revenue (£173k) drastically below Expected Revenue (£551k), resulting in a £193.21k direct loss tied to operational failures.

> The payer mix is led by Credit Card (£201k), followed closely by Insurance (£182k) and Cash (£168k), showing a reliance on direct patient payments.

> MedCare Plus is the dominant insurer, responsible for £241.09k in costs, making them the most financially important third-party partner.

### Service Costs: High-Value Procedures
Top Cost Treatments: The most expensive treatments on average are MRI () and Physio ().
Treatment Ranking: The average cost per treatment type is: MRI Physio Chemo ECG X-Ray.

### Key Takeaway 
> The most critical issue the dashboard reveals is the operational inefficiency driven by high cancellation and no-show rates. Addressing this is paramount, as it's the likely root cause of the gap between Expected () and Actual () Revenue.












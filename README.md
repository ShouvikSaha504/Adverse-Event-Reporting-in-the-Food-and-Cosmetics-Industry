# Adverse-Event-Reporting-in-the-Food-and-Cosmetics-Industry
A Case Study on Adverse Event Reporting in the Food and Cosmetics Industry by FDA - Power BI


## Industry Context

The Food and Drug Administration (FDA) is crucial in safeguarding the food and beverage sector by monitoring and regulating product safety. Data analysis is vital in identifying and mitigating risks related to adverse events. Historical incidents, such as the lead contamination in Maggi noodles and undeclared allergens in Patanjali products, underscore the ongoing challenges in ensuring food safety. The CAERS (CFSAN Adverse Event Reporting System) database serves as a pivotal resource for tracking and analyzing adverse events and product complaints related to foods, dietary supplements, and cosmetics.

## Objective

The primary objectives of this analysis were to:

- **Develop a comprehensive Power BI dashboard**: To visualize adverse event data in the food and beverage industry systematically.
- **Identify trends and patterns**: To analyze key parameters such as gender, age, product types, and symptoms.
- **Enhance industry safety standards**: By providing actionable insights to improve risk management and regulatory compliance.

## Methodologies

### Data Source

The dataset used for this analysis is from the [CAERS_ASCII_2004_2017Q2.csv](https://github.com/ShouvikSaha504/Adverse-Event-Reporting-in-the-Food-and-Cosmetics-Industry/blob/5dd27c6b31c6786cd2aa771ae5278ee8efb08a1c/CAERS_ASCII_2004_2017Q2.csv), which includes detailed records from the FDA's adverse event reporting system covering:

1. **RA_Report #**: Unique identifier for each adverse event report.
2. **RA_CAERS Created Date**: Date when the report was entered into the CAERS database.
3. **AEC_Event Start Date**: Date when the adverse event started.
4. **PRI_Product Role**: Role of the product (e.g., suspect or concomitant).
5. **PRI_Reported Brand/Product Name**: Name of the product associated with the adverse event.
6. **PRI_FDA Industry Code & Name**: Categorization of the product based on FDA codes and names.
7. **CI_Age at Adverse Event**: Age of the individual experiencing the adverse event.
8. **CI_Age Unit**: Unit of measurement for age.
9. **CI_Gender**: Gender of the individual.
10. **AEC_One Row Outcomes**: Outcomes of the event (e.g., hospitalization).
11. **SYM_One Row Coded Symptoms**: Symptoms reported in association with the adverse event.

### Data Preprocessing

To prepare the data for analysis:

- **Identified and imputed missing values**: Addressed inconsistencies and grouped entries by industry code for accuracy.
- **Consolidated age data**: Combined numerical values and units into a standardized column using DAX queries.
- **Performed string manipulations**: Standardized categorical columns for uniformity.
- **Cleaned data entries**: Removed or corrected improper entries to ensure high data quality.

### Part 1: Data Cleaning, Modeling, and DAX in Power BI

1. **Data Importing and Preliminary Analysis**: Import and examine the dataset in Power BI.
2. **Handling Missing Values**: Address missing values and apply appropriate strategies.
3. **Data Type Standardization**: Ensure correct data types for dates and numerical fields.
4. **Product Role Categorization**: Analyze distribution based on product roles.
5. **FDA Industry Analysis**: Group and analyze data by FDA industry codes.
6. **Age Group Analysis**: Create and analyze age groups from age data.
7. **Gender-Based Analysis**: Examine adverse event reports by gender.
8. **Adverse Event Start Date Analysis**: Identify trends over time.
9. **Outcome Categorization**: Categorize and analyze adverse event outcomes.
10. **Symptom Frequency Analysis**: Analyze the frequency of reported symptoms.
11. **Correlation between Age and Symptom Types**: Investigate correlations using DAX.
12. **Industry and Outcome Relationship**: Examine relationships between industry codes and outcomes.
13. **Time Series Analysis of Reports**: Identify seasonal trends in report submissions.
14. **DAX for Advanced Age Analysis**: Calculate average, median, and mode of ages at which events occur.
15. **Product Name Analysis**: Identify commonly reported products.
16. **Geographical Distribution (If Applicable)**: Analyze distribution by region, if available.
17. **Advanced DAX: Report Frequency Calculation**: Calculate report frequency per month or year.
18. **Symptom Severity Index**: Create an index for symptom severity.
19. **Report Duplication Analysis**: Identify and handle duplicate reports.
20. **Predictive Modeling for Adverse Event Risk**: Develop a predictive model using DAX.
21. **Complex Symptom Pattern Analysis**: Analyze patterns in symptom co-occurrence using nested DAX functions.
22. **Advanced Outcome Prediction Model**: Create a model to estimate the likelihood of severe outcomes.

### Part 2: Dashboard Building

1. **Adverse Event Reporting Dashboard**: Develop a dashboard showcasing key metrics with interactive filters.
2. **Dashboard Design and Accessibility**: Ensure the dashboard is visually appealing and user-friendly.
3. **Time-Based Reporting Trends**: Visualize trends in reporting over time.
4. **Industry and Outcome Correlation Visualization**: Create visualizations showing correlations between industries and outcomes.
5. **Demographic Analysis Section**: Analyze age and gender distributions.
6. **Key Insights and Data Storytelling**: Summarize insights and trends with visual storytelling.

### Dashboard:
[**Dashboard Link**](https://github.com/ShouvikSaha504/Adverse-Event-Reporting-in-the-Food-and-Cosmetics-Industry/blob/3903cb4498f60d1f03b2060f2776246c2b15ef00/Dashboard.pbix)

### Dashboard Snap:
![Dashboard Snap](https://github.com/user-attachments/assets/fde0e86c-72ee-402c-a863-7a7d72915a58)



## Insights & Actionable Items

The preprocessed dataset contains approximately **34,000 rows** and **18 columns**. Key insights from the Power BI dashboard include:

- **Disproportionate impact on demographics**: **23,000 female-related adverse events** were noted.
- **Age group analysis**: The **36-50 years** age group had the highest frequency of adverse events.

These findings suggest a need for targeted education programs, particularly for females in the 36-50 age group, to improve awareness and safety.

---

For further details or to access the project files, please refer to the [dataset link]([https://prod-files-secure.s3.us-west-2.amazonaws.com/d1e1bc70-9ede-4c69-84fd-42c5605803a0/f005446a-14f3-426e-b31e-03df53eb3d89/CAERS_ASCII_2004_2017Q2.csv](https://github.com/ShouvikSaha504/Adverse-Event-Reporting-in-the-Food-and-Cosmetics-Industry/blob/5dd27c6b31c6786cd2aa771ae5278ee8efb08a1c/CAERS_ASCII_2004_2017Q2.csv)) or contact me directly.


# FDA Adverse-Event-Reporting-in-the-Food-and-Cosmetics-Industry
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

In Part 1 of the analysis, the focus is on data cleaning, modeling, and the application of DAX in Power BI. The process begins with importing and examining the dataset, addressing missing values, and ensuring data type standardization for dates and numerical fields. Product roles are categorized to analyze their distribution, and FDA industry codes are grouped for detailed analysis. Age and gender data are examined to create relevant age groups and understand gender-based trends. The adverse event start dates are analyzed to identify temporal trends, and outcomes are categorized for further analysis. Symptom frequency is reviewed, and correlations between age and symptom types are investigated using DAX. Relationships between industry codes and outcomes are explored, while time series analysis helps identify seasonal trends. Advanced DAX techniques are used to calculate age statistics, report frequencies, and symptom severity. Product names are analyzed to identify common issues, and if geographical data is available, regional distribution is examined. The analysis also includes detecting and handling duplicate reports, developing predictive models for adverse event risks, and creating complex models for symptom patterns and outcome predictions using nested DAX functions.






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

## Conclusion

In conclusion, the analysis of adverse events in the food and cosmetics industry, utilizing the CAERS dataset and Power BI, has provided valuable insights into the patterns and trends of reported incidents. The comprehensive data cleaning and modeling process, combined with advanced DAX calculations, has enabled a thorough examination of key factors such as product roles, age and gender demographics, and symptom frequencies. The findings reveal significant trends, including disproportionate impacts on certain demographics and frequent issues associated with specific products. By identifying correlations between age, symptoms, and industry codes, and by analyzing seasonal variations in report submissions, the project highlights critical areas for targeted intervention and risk management. The development of predictive models and advanced analyses further equips industry stakeholders with actionable insights to enhance safety standards and regulatory compliance. Ultimately, this analysis underscores the importance of ongoing vigilance and data-driven approaches in safeguarding public health within the food and cosmetics sectors.

---

For further details or to access the project files, please refer to the [dataset link]([https://prod-files-secure.s3.us-west-2.amazonaws.com/d1e1bc70-9ede-4c69-84fd-42c5605803a0/f005446a-14f3-426e-b31e-03df53eb3d89/CAERS_ASCII_2004_2017Q2.csv](https://github.com/ShouvikSaha504/Adverse-Event-Reporting-in-the-Food-and-Cosmetics-Industry/blob/5dd27c6b31c6786cd2aa771ae5278ee8efb08a1c/CAERS_ASCII_2004_2017Q2.csv)) or contact me directly.


# **Excel_Project-Job_Postings_Data_Analytics**

 **My project showcasing my Excel skills**   

 # Part 1  
 
 ## **Salary Dashboard**
 ![Salary_Dashboard_Full](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/Salary_Dashboard_Full.PNG)

 ## **Salary Analysis**
 
## **Introduction**

This interactive salary analytics dashboard was developed to empower data job seekers and professionals in benchmarking compensation across roles, geographies, and skill sets.

The dataset originates from an applied Excel-based data analysis course and encompasses structured information on:

👨‍💼 Job Titles

💰 Compensation (Annual Salaries)

📍 Geographic Locations

🛠️ Technical Skill Requirements

This dashboard leverages Excel as a Business Intelligence (BI) tool, showcasing the integration of formulas, data modeling, visualization, and data validation techniques to derive actionable insights.

## **Dashboard File**
The Final dashboard is in [Part_1-Salary_Dashboard](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Part_1-Dashboard/Part_1-Salary_Dashboard.xlsx)

## **Excel Competencies Applied**

📉 Data Visualization: Bar charts, map charts, interactive visuals.

🧮 Analytical Functions: Array formulas, conditional filtering, median calculations.

❎ Data Quality Controls: Validation lists to enforce integrity and consistency.


## **Dataset Information**
The dataset utilised in this work comprises real world data science job information from 2023. It is sourced from my Excel training program, which serves as a foundational resource for developing analytical proficiency using Microsoft Excel.

The dataset encompasses comprehensive details on the following key attributes:

**👨‍💼 Job Titles:** Roles and designations across diverse organiations.  
**💰 Salaries:** Compensation ranges and renumeration insights.  
**📍 Locations:** Geographic distribution of job opportunities.  
**🛠️ Skills:** Core and technical competences required in the field.

## **Dashboard build**  

###  📉 **Charts**  
#### 📊 **Compensation Analysis by Job Title – Bar Chart**   
![Data_Science_Job-Bar_Chart](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/Data_Science_Job-Bar_Chart.png)  

🛠️ Feature Used: Custom bar charts with formatted salary values.  

🎨 Visualization Design: Horizontal orientation for quick cross-role comparison.  

📉 Data Treatment: Roles ranked in descending order of median salary.  

💡 Key Insight: Senior and engineering roles command higher compensation compared to analyst positions.  

#### 🗺️ **Geographic Median Pay Benchmarking – Map Chart**  
![Country_Median_Salary_Distribution-Map_Chart](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/Country_Median_Salary_Distribution-Map_Chart.PNG)

🛠️ Feature Used: Excel map chart for geospatial salary distribution.

🎨 Design Choice: Color gradient encoding to reflect compensation tiers.

📊 Analytical Representation: Median salaries aggregated by country.

💡 Key Insight: Regional disparities are immediately visible, spotlighting high-earning vs. low-earning markets.  

## 🧮 **Advanced Formulas & Functions**  
#### 💰 **Median Salary by Role & Region**  
***
=MEDIAN(  
IF(  
    (jobs[job_title_short]=A2)*  
    (jobs[job_country]=country)*  
    (ISNUMBER(SEARCH(type,jobs[job_schedule_type])))*  
    (jobs[salary_year_avg]<>0),  
    jobs[salary_year_avg]  
)  
)
***  
🔍 Multi-Dimensional Filtering: Conditional logic across job title, geography, and schedule type.  
📊 Array Calculation: Dynamic computation of median salary across subsets.  
🎯 Actionable Output: Delivers tailored salary benchmarks by role, country, and contract type.  

#### 🍽️ **Background Table**  
![Background_Table_1](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/Background_Table_1.PNG)  

#### 📉 **Dashboard Implementation**  
![Dashboard_Implementation-Job_Title_Bar_Xhart](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/Dashboard_Implementation-Job_Title_Bar_Chart.PNG)  

#### ⏰ **Unique Job Schedule Types**  
***  
=FILTER(J2#,(NOT(ISNUMBER(SEARCH("and",J2#))+ISNUMBER(SEARCH(",",J2#))))*(J2#<>0))  
***  
🔍 Deduplicated List Creation: Excludes ambiguous or invalid entries.  
📊 Data Cleaning Mechanism: Ensures accurate categorization of job schedule types.  
🎯 Result: A curated list for downstream use in dashboard filters.  

#### 🍽️ **Background Table**  
![Background_table_2](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/Backgrpond_table_2.PNG)  

#### 📉 **Dashboard Implementation**  
![Dashboard_Implementation-Job_Type](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/Dashboard_Implementation-Job_Type.PNG)  

❎ Data Validation Integration

🔒 Controlled Inputs: Applied to Job Title, Country, and Type fields.

🚫 Error Prevention: Blocks inconsistent or non-standard user entries.

👥 Enhanced UX: Ensures a clean, reliable interactive dashboard experience.  

![Salary_Dashboard-Job_Title](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/Salary_Dashboard-Job_Title.PNG)  

### **Conclusion** 

The Excel Salary Dashboard provides an end-to-end demonstration of how data wrangling, statistical analysis, and visualization converge to inform compensation decisions.

By leveraging Excel’s BI capabilities, users can:

📍 Benchmark salaries across countries  

👨‍💼 Compare compensation by job title  

⏰ Assess pay trends by schedule type  

This enables evidence-based career planning and highlights how location and role specialization directly influence salary outcomes.






 

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


# Part 2  
# Analysis Report  
## Summary
This comprehensive analytical study investigates the data science employment landscape, focusing on compensation structures, skill requirements, and geographical salary distributions. Through systematic quantitative analysis of real-world job market data, this research identifies key determinants of compensation levels and establishes correlations between technical competencies and earning potential within the data science domain.  

### Research Objectives  
This investigation addresses four critical research questions designed to provide actionable intelligence on the data science job market:  
1. Does skill diversity correlate positively with compensation levels?  
2. What geographic variations exist in data science role compensation?  
3. Which technical competencies demonstrate highest market prevalence among data professionals?  
4. What compensation ranges are associated with the most in-demand technical skills?  

### Analytical Methodology  
#### Technical Stack  
The following analytical frameworks and tools were deployed throughout this investigation:

-**📊Pivot Tables:** For multidimensional data aggregation and cross-tabulation analysis.  
-**📈Pivot Charts:** For visual representation of complex datasets and trend identification.  
-**🧮DAX (Data Analysis Expressions):** For creating custom calculated measures and KPIs.  
-**🔍Power Query:** For ETL (Extract, Transform, Load) operations and data cleansing workflows.  
-**💪Power Pivot:** For relational data modeling and establishing table relationships.  

### Dataset Specification  
#### Data Provenance  
The analytical dataset comprises empirical job posting data from the 2023 calendar year, sourced from multiple job aggregation platforms. The dataset exhibits the following dimensional characteristics:  

Key Attributes:

-**👨‍💼Job titles**  
-**💰Salaries**  
-**📍Locations**  
-**🛠️Skills**  


## Analysis 1: Skill Diversity and Compensation Correlation (Do more skills get you better pay?)  

### Skill: Power Query (ETL)  

#### Extract Phase  
A dual-query extraction strategy was implemented using Power Query on data_salary_all.xlsx:  
Query 1: Comprehensive job postings dataset extraction 
Query 2: Normalized skills dimension table with many-to-many relationship to job ID.    

#### Transform Phase  
The transformation layer incorporated multiple data quality operations:  
Schema validation and data type enforcement
Dimensional reduction through column elimination of non-analytical fields
Text normalization including pattern-based string removal
Whitespace standardization across all text fields  

-📊 data_job_all:  
![data_jobs_all_as](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/data_jobs_all_as.PNG)  

Skills taxonomy standardization
Removal of duplicate skill entries per job posting
String cleaning and formatting consistency

-🛠️ data_job_skills:  
![data_job_skills_as](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/data_job_skills_as.PNG)  

### 🔗 Load Phase  
Both transformed datasets were loaded into the Excel data model, establishing the foundation for the analytical layer:  

-📊 data_jobs_all: Primary fact table containing job-level metrics  
![data_jobs_all](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/data_jobs_all.PNG)  

-🛠️ data_job_skills: Dimension table for skills attribution  
![data_job_skills](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/data_job_skills.PNG)  

###  📊  Statistical Analysis
#### 💡 Key Findings  

Positive Correlation Identified: A statistically significant positive correlation exists between skill count per job posting and median annual compensation, with the strongest relationship observed in Senior Data Engineer and Data Scientist role classifications.
Compensation Stratification: Role categories requiring limited skill sets (e.g., Business Analyst positions) demonstrate substantially lower median compensation levels, indicating market premium for specialized, multi-competency profiles.  

![Insight_1](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/Insight_1.PNG)  

#### 🤔 Strategic Implications  
The observed correlation between skill portfolio breadth and compensation emphasizes the economic value of continuous skill acquisition and cross-functional competency development. Professionals targeting upper-quartile compensation bands should prioritize developing complementary technical skill sets rather than single-domain expertise.  

## Analysis 2: Geographic Compensation Distribution (What’s the salary for data jobs in different regions?)  
### Analytical Framework: Pivot Tables & DAX Measures  

#### Pivot Table Construction  
A multidimensional pivot table was constructed utilizing the integrated data model with Power Pivot:  
Row Dimension: job_title_short for role classification  
Value Aggregation: salary_year_avg with custom median calculation
Added new Measure: Geographic filter for US market median Salary Cakculation.  

### DAX Measure for US Market Segmentation:  
***
=CALCULATE(
    MEDIAN(data_jobs_all[salary_year_avg]),
    data_jobs_all[job_country] = "United States")
 ***  
#### DAX Implementation for Salary Metrics
A reusable calculated measure was created for median salary computation:  
***
Median Salary := MEDIAN(data_jobs_all[salary_year_avg])  
***  
### Comparative Geographic Analysis  
#### 💡 Key Findings

**Premium for Senior Technical Roles:** Senior Data Engineer and Data Scientist positions command elevated median compensation in both domestic (US) and international markets, reflecting global demand for advanced analytical expertise.  
**Geographic Compensation Differential:** Substantial salary variance exists between US and non-US markets, particularly pronounced in high-specialization technical roles. This disparity correlates with the concentration of technology sector organizations and venture capital investment within the United States.  

![Insight_2](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/Insight_2.PNG)

#### 🤔 Strategic Implications  
These geographic compensation insights provide critical intelligence for both career planning and organizational talent acquisition strategies. Understanding regional compensation benchmarks enables data professionals to optimize location decisions and empowers organizations to structure competitive compensation packages aligned with market dynamics.  

## Analysis 3: Market-Dominant Technical Competencies (What are the top skills of data professionals?)  
### Data Modeling: Power Pivot Implementation
***-Relational Data Model Construction***
A star schema data model was engineered through Power Pivot integration:  
Fact Table: data_jobs_all containing measures and foreign keys  
Dimension Table: data_jobs_skills providing skills taxonomy  
Relationship Type: One-to-many cardinality between jobs and skills  

Entity Relationship Configuration  
-A primary key/foreign key relationship was established using job_id as the common dimension, enabling seamless cross-table aggregations and filtering.  

![Data_Model](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/Data_Model.PNG) 

Power Pivot Interface Utilization
The Power Pivot management interface facilitated data model refinement, measure creation, and relationship validation.  

![Power_pivot_menu](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/Power_pivot_menu.PNG)  

### Skills Frequency Analysis  
#### 💡 Key Findings  

**Foundational Language Dominance:** SQL and Python demonstrate overwhelming market prevalence across data-centric roles, confirming their status as essential competencies for data manipulation, transformation, and analytical programming.  
**Cloud Infrastructure Emergence:** Cloud platforms including AWS (Amazon Web Services) and Azure exhibit significant market penetration, reflecting the industry-wide migration toward distributed computing architectures, scalable data storage solutions, and cloud-native analytics platforms.

![Insight_3](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/Insight_3.PNG)  

#### 🤔 Strategic Implications  
The prevalence distribution of technical skills provides directional guidance for professional development roadmaps and curriculum design. Data professionals must prioritize core competencies (SQL, Python) while simultaneously developing proficiency in emerging cloud technologies to maintain competitive positioning in the talent marketplace.  

## Analysis 4: Skill-Based Compensation Analysis (What’s the pay of the top 10 skills?)  
### Visualization: Advanced Pivot Chart Construction
Dual-Axis Combination Chart
A composite visualization was engineered to simultaneously represent two key metrics:

**Primary Y-Axis:** Median annual compensation (Clustered Column chart type)  
**Secondary Y-Axis:** Skill likelihood percentage (Line with Markers chart type)  

#### Chart customization included:

Descriptive title and axis labels for clarity
Removal of gridlines to reduce visual clutter
Diamond marker styling for skill likelihood trajectory
Color-coded series for metric differentiation

### Compensation-Skill Value Analysis  
#### 💡 Key Findings  

High-Value Technical Skills: Python, Oracle, and SQL command the highest median compensation levels, signaling their critical importance in high-value technical positions and their direct correlation with specialized data engineering and analytics roles.
Low-Specialization Skill Gap: Generalist productivity tools (PowerPoint, Word) demonstrate both minimal median compensation and low market likelihood, indicating limited differentiation value and reduced demand in specialized, high-compensation segments.

![Insight_4](https://github.com/Ejiole-C/Excel_Project-Job_Postings_Data_Analytics/blob/main/Resources/Insight_4.PNG)  

#### 🤔 Strategic Implications  
This analysis quantifies the return on investment for technical skill acquisition. The data unambiguously demonstrates that proficiency in programming languages (Python, SQL) and database technologies (Oracle) yields substantial compensation premiums. Professionals seeking to maximize earning potential should strategically allocate learning investments toward these high-value competencies rather than general-purpose business tools.  

## Conclusions and Recommendations  
This systematic investigation of the data science employment landscape leveraged Excel's advanced analytical capabilities—including Power Query for ETL workflows, Power Pivot for dimensional modeling, DAX for custom metrics, and dynamic visualization through PivotCharts—to extract actionable insights from empirical job market data.  

### Principal Findings  
The analysis establishes clear quantitative relationships between:  

Skill portfolio breadth and compensation levels, with multi-skilled profiles commanding significant salary premiums
Geographic location and market rates, revealing substantial US/non-US compensation differentials
Technical competency mix and market demand, identifying SQL, Python, and cloud platforms as dominant requirements
Specific skill proficiencies and earning potential, quantifying the compensation advantage of programming and database expertise  

### Practical Applications  
This research serves as an evidence-based framework for data professionals navigating career development decisions, organizations benchmarking compensation structures, and educational institutions designing curriculum to align with market demands. The identified skill-compensation relationships provide clear directional guidance for maximizing career trajectory and earning potential within the data science domain.







 

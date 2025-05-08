# IS-5960-03-MRP
Employability analytics Tool HireEdge

Project Overview:
This project involved building an interactive Employability Analytics Dashboard using Power BI. 
The goal was to help job seekers and consultants explore job market trends, salary insights, skill demands, and location-based job opportunities.
The dataset was cleaned and transformed using Power Query (M Language), and insights were derived using DAX calculations in Power BI.
Data Collection : 
The dataset is collected from Kaggle .

Data Cleaning and Transformation (Power Query M Code):
Using Power Query M Code, a number of transformation procedures were conducted to guarantee the dataset was correct, clean, and prepared for analysis. Key columns' data types were first changed: experience_level and employment_type were changed to text, while salary and salary_USD were changed to numeric kinds. This guarantees constant text filtering and precise numerical computation. To keep results from being skewed by invalid entries, rows with blank or missing job_title values were eliminated.
Incorrect entries in the salary_currency column, such as the misspelling "US Dollars," were fixed and standardized to "USD". Negative salary values were discovered and converted to absolute values, with the assumption that they indicated data entry errors rather than true negative incomes. To ensure dataset completeness, items with null values in experience_level were assigned the default value of "Entry Level".
To standardize the experience_level column further, frequent acronyms were expanded to full descriptions—for example, "EN" was replaced with "Entry Level", "MI" with "Mid Level", "SE" with "Senior Level", and "EX" with "Executive Level". Additionally, job titles were cleaned by removing leading and trailing white spaces to ensure uniformity in grouping and aggregate during analysis.

DAX Measures for Analytical Insights:
Power BI employed a variety of DAX measures to examine job and salary data. Basic metrics, such as the total number of jobs and the average, maximum, and minimum salaries in USD, were computed. Employment types (Full-Time, Freelance, Contract) and unique job titles were analyzed using filtered counts and DISTINCTCOUNT. For time-based trends, month names were converted to numerical values using SWITCH, and AVERAGEX offered insights into salaries by experience level.

PowerBI Dashboard- HIREEDGE:

1. The Power BI dashboard includes five pages: Homepage, Opportunities Summary, Hiring Trends, Salary Insights, and Jobs in MO.
2. Each page features interactive elements such as slicers, KPI cards, and various visuals (bar, line, donut, matrix).
3. Filterable tables are used throughout to allow dynamic exploration of job data.
4. Insights highlight job demand by category, experience level, salary trends, and work setting preferences.
5. Location-based job opportunities are visualized to assist both job seekers and consultants in decision-making.

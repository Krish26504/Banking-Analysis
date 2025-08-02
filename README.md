# Banking-Analysis
BankEDA: Exploratory Data Analysis on Bank Customer Data
Tools Used: Python, SQL, SQLite3, Pandas, Seaborn, Matplotlib, SciPy

📌 Project Overview
This project performs an end-to-end Exploratory Data Analysis (EDA) on banking customer data using SQL and Python. The goal is to uncover insights into customer demographics, deposit behavior, and campaign effectiveness. Both SQL and Python (with libraries like Pandas and Seaborn) are used to complement each other for faster querying and visualizations.

Aims
Perform SQL-powered queries using SQLite3 to extract structured insights.

Conduct in-depth EDA using Pandas and Seaborn for feature distributions, correlation analysis, and customer segmentation.

Use statistical testing (SciPy) to evaluate the influence of features on term deposit subscription.

Support business decisions by identifying patterns in customer responses and campaign strategies.

Dataset
The dataset contains records of a bank’s marketing campaigns. Key columns include:

age, job, marital, education, balance

default, housing, loan, contact, campaign

previous, pdays, duration, poutcome

deposit (target variable: yes/no)

How to Run the Project
Requirements
Install the following Python packages:

bash
Copy
Edit
pip install pandas seaborn matplotlib scipy sqlite3
Steps 
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/BankEDA.git
cd BankEDA
Open the notebook:

bash
Copy
Edit
jupyter notebook "BankEDA (Version 2).ipynb"
Follow the code cells for:

SQLite3 database creation & querying

Data cleaning and transformation using Pandas

Statistical analysis

Visualizations using Seaborn and Matplotlib

SQL Analysis Highlights
Created SQLite3 tables and performed queries like:

sql
Copy
Edit
SELECT job, COUNT(*) AS customers
FROM bank_data
GROUP BY job
ORDER BY customers DESC;
Analyzed key relationships:

Housing loan status vs. deposit subscription

Contact type performance (cellular vs telephone)

Campaign duration vs. outcome

Joined tables and filtered using WHERE, GROUP BY, and aggregate functions.

Visual EDA (Python)
Distribution plots of age, balance, duration

Bar plots for categorical columns like job, education, and contact

Heatmap of feature correlations

Pie chart showing deposit conversion rate

Campaign success rate by month and previous contact status

Statistical Testing
Used Chi-square tests to check independence of variables like job, education, housing, and deposit.

Applied correlation tests to numeric features like age, balance, and duration.


Customers contacted via cellular were more likely to subscribe to deposits.

Higher balance customers showed higher deposit conversion.

Duration of call is highly correlated with positive outcome — but should be treated carefully (leakage).

Customers previously contacted (in past campaigns) had a higher success rate.

Jobs like “admin.” and “technician” are common, but “retired” and “student” had higher subscription rates.

Conclusion
Combining SQL and Python gave a flexible and scalable way to analyze the bank’s customer data. This project can help marketing teams:

Identify target demographics

Optimize campaign strategies

Make data-driven decisions based on real behavior patterns

Files Included
BankEDA (Version 1).ipynb – initial version of the project

BankEDA (Version 2).ipynb – cleaned, optimized version with refined insights and better structure
Home
<img width="1280" height="720" alt="Home (1)" src="https://github.com/user-attachments/assets/493ae66f-8365-4211-9a70-ce73b365d450" />
Summary
<img width="1280" height="720" alt="Summary" src="https://github.com/user-attachments/assets/241eac72-d7e1-4cb8-b4ff-7c6ebbb7a09c" />
Loan Analysis
<img width="1280" height="720" alt="Loan Analysis" src="https://github.com/user-attachments/assets/9eec2394-2915-4e1d-b4ce-ea34d4f57d78" />




bank_data.sqlite – SQLite database created and queried inside the notebook

README.md – documentation of the project (this file)

👨‍💻 Author
Krish Raj Anand

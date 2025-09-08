# 📊 Customer Churn Analysis and Prediction 

## 📌 Overview

This project is an end-to-end churn analysis for a telecom firm, designed to understand customer attrition, predict future churners, and provide actionable insights for customer retention strategies. 

It uses a combination of SQL, Power BI, and machine learning to build a comprehensive solution.

In today’s competitive business landscape, retaining customers is vital for long-term success, and churn analysis is a key technique for achieving this.

---

## 🎯 Project Goals

***Visualize and Analyze Customer Data:*** 
Explore customer data at different levels, including demographic, geographic, payment and account information, and services.

***Study Churner Profiles:*** 
Identify characteristics of customers who have churned to help in designing targeted marketing campaigns.

***Predict Future Churners:*** 
Develop a method to predict which customers are at risk of leaving.

---

## 🔎 Methodology
This project follows a multi-step process, from data extraction to visualization and predictive modeling.

**1. ETL Process in SQL Server:**

- An ETL (Extract, Transform, Load) framework was created to handle the customer data.
- Data was imported from a CSV source file into a staging table using the SQL Server Import Wizard.
- Data exploration was performed to check for distinct values and nulls.  
- Null values were removed, and the cleaned data was loaded into a production table.
- Views were created to facilitate data loading into Power BI for analysis.

**2. Data Modeling and Visualization (Power BI):**

- Customer data was connected to Power BI to create an interactive dashboard.
- Custom columns were added to categorize data, such as
- Churn Status and ranges for Monthly Charge, Age, and Tenure.
- Key metrics were calculated, including
- Total Customers, New Joiners, Total Churn, and Churn Rate.
- Visualizations were created to show a summary of key metrics, demographic and account information, and a churn distribution analysis.

**3. Churn Prediction (Machine Learning):**

- A Random Forest machine learning algorithm was used to predict customer churn. This algorithm was chosen for its robustness and accuracy in classification tasks.
- Data was prepared by dropping irrelevant columns and encoding categorical variables.
- The data was split into training and testing sets to train and evaluate the model.
- The trained model was then used to predict potential churners among new joiners.

---

## 🛠️ Tools and Technologies

- **Microsoft SQL Server:** Used for the ETL process, data cleaning, and data warehousing.
- **Power BI:** Utilized for data visualization and creating the interactive dashboard.
- **Jupyter Notebook (Python):** Employed for the machine learning model development.
- **Libraries:** pandas, numpy, matplotlib, seaborn, and scikit-learn were used for data manipulation, visualization, and machine learning.

---

## 📈 Key Findings & Insights

- **Dashboard Summary:** The dashboard provides a high-level overview, showing a total of 6,418 customers, with 411 new joiners and 1,732 churned customers, resulting in a churn rate of 27.0%.

<img width="1160" height="650" alt="Dashboard_Screenshot_1" src="https://github.com/user-attachments/assets/b52bece5-d0bf-49f5-9358-4b7eff6e52cf" />


<img width="1162" height="651" alt="Dashboard_Screenshot_2" src="https://github.com/user-attachments/assets/8b0c3f68-3304-4085-b9e8-10b050e7457d" />


- **Demographic Analysis:** The project includes visuals for churn rates based on gender and age groups.
  
- **Account and Service Analysis:** Insights were gained by analyzing churn rates related to payment methods, contract types, and specific services like internet or streaming options.

- **Predictive Model:** The Random Forest model successfully predicted future churners, providing a list of at-risk customers who can be targeted with proactive retention campaigns.

---

## How to Use This Repository

This repository is structured to allow you to follow the project's steps. You can review the SQL queries for the ETL process, the data transformation steps in Power BI, and the Python code for the machine learning model. The project's methodology can be applied to other industries that value customer retention, such as retail, finance, and healthcare.



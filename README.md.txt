# Insurance Customer Risk and Cost Analysis

## Project Overview

This project explores how different customer characteristics influence health insurance costs. The goal is to better understand risk factors that drive insurance charges and demonstrate how data analysis can support decision making in the insurance industry.

Insurance companies rely heavily on data to assess risk, determine pricing, and manage financial exposure. By analyzing customer attributes such as smoking habits, age, body mass index (BMI), and geographic location, insurers can better understand which groups are more likely to generate higher healthcare costs.

This project uses a real world dataset to examine these relationships and present the findings through clear visualizations and structured analysis.

The analysis was performed using SQL and Power BI, while GitHub was used to document and present the project.

---

## Data Source

The dataset used in this project comes from Kaggle.

Source:  
https://www.kaggle.com/datasets/mirichoi0218/insurance

The dataset contains information about 1,338 insurance customers, including demographic and health related attributes that may influence insurance charges.

Key fields in the dataset include:

- Age of the customer
- Gender
- Body Mass Index (BMI)
- Number of children covered by insurance
- Smoking status
- Region of residence
- Medical insurance charges

---

## Business Objective

Insurance companies must accurately estimate healthcare risk in order to set fair premiums and maintain financial stability.

This project explores the following questions:

- Which customer characteristics are most strongly associated with higher insurance costs?
- How much more expensive are smokers compared to non smokers?
- Do age and body weight influence healthcare charges?
- Are there regional differences in insurance costs?

Understanding these patterns helps insurers design pricing strategies and identify high risk groups that may require additional monitoring.

---

## Tools and Technologies Used

- SQLite for storing and querying the dataset
- SQL for performing analytical queries
- Power BI for building the data visualization dashboard
- GitHub for project documentation and version control

---

## Dataset Overview

The dataset contains 1,338 insurance customers.

Each record represents a customer and their associated healthcare insurance cost.

Customer attributes analyzed include:

- Age group
- Smoking status
- BMI category
- Geographic region

These attributes were grouped and analyzed to understand how they influence average insurance charges.

---

## Key Findings

### Smoking Status

Smoking is the strongest predictor of high insurance costs in the dataset.

| Smoking Status | Average Insurance Charge |
|---|---|
| No | 8,434 |
| Yes | 32,050 |

Smokers generate nearly four times higher healthcare costs than non smokers. This reflects the increased medical risks associated with smoking.

---

### Age Groups

Healthcare costs increase steadily with age.

| Age Group | Average Charge |
|---|---|
| 18–29 | 9,182 |
| 30–39 | 11,738 |
| 40–49 | 14,399 |
| 50+ | 17,902 |

Older customers tend to require more medical care, which leads to higher insurance claims and overall charges.

---

### BMI Categories

Body Mass Index also influences insurance costs.

| BMI Category | Average Charge |
|---|---|
| Underweight | 8,852 |
| Normal | 10,409 |
| Overweight | 10,987 |
| Obese | 15,552 |

Customers classified as obese generate significantly higher medical costs compared to other BMI groups.

---

### Geographic Region

Average insurance charges vary slightly by region.

| Region | Average Charge |
|---|---|
| Southeast | 14,735 |
| Northeast | 13,406 |
| Northwest | 12,417 |
| Southwest | 12,346 |

While regional differences exist, they are smaller compared to the effects of smoking and BMI.

---

## Combined Risk Analysis

To better understand how multiple factors interact, the analysis also examined smoking status alongside BMI risk groups.

| Smoking Status | BMI Risk Group | Avg Charge | Customers |
|---|---|---|---|
| Yes | Obese | 41,557 | 145 |
| Yes | Not Obese | 21,363 | 129 |
| No | Obese | 8,842 | 562 |
| No | Not Obese | 7,977 | 502 |

The results show that customers who both smoke and are obese generate extremely high insurance costs. This group represents the highest risk category in the dataset.

---

## Dashboard

The findings were visualized using a Power BI dashboard to make the results easier to interpret for business stakeholders.

The dashboard highlights:

- Average insurance charges by smoking status
- Average insurance charges by age group
- Average insurance charges by region

Dashboard Preview

![Insurance Dashboard](dashboards/insurance_risk_dashboard.png)

---

## Business Insights

Several important insights emerge from the analysis:

- Smoking is the most significant driver of high insurance costs.
- Age is strongly correlated with increasing healthcare expenses.
- Higher BMI categories are associated with greater insurance charges.
- Regional differences exist but are less influential compared to lifestyle and health factors.

These insights can help insurance providers refine pricing models and better understand customer risk profiles.

---

## Project Structure

insurance-risk-analysis-project
│
├── data
│   insurance.csv
│
├── dashboards
│   insurance_risk_dashboard.png
│   insurance-risk-analysis-dashboard.pbix
│
├── sql
│   insurance_analysis_queries.sql
│
└── README.md

---

## Author

Kayode Alatise  
Data Analyst | Data Governance | Business Intelligence | Data Science
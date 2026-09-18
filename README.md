# Bank Transaction Churn Prediction & Risk Analytics

## 📌 Business Overview
Customer churn and fraud detection are critical challenges in the financial services sector. This project builds an end-to-end predictive and exploratory data analytics pipeline using a dataset of **550,000 retail banking transactions (2019-2024)**. By processing transactional features like transaction hours, credit scores, and account types, this project enables financial institutions to segment customers, perform **RFM (Recency, Frequency, Monetary) value modeling**, and deploy proactive retention strategies before churn occurs.

## 🛠️ Data & Technical Toolbox
* **Core Analytics Platform:** [R Tooling](https://r-project.org) using `tidyverse`, `readxl`, and `lubridate`
* **Machine Learning Pipeline:** [Tidymodels Framework](https://tidymodels.org) including `rsample`, `recipes`, `parsnip`, and `workflows`
* **Class Imbalance Handling:** [Themis Package](https://r-project.org) (`step_smote`) to optimize heavily skewed fraud profiles
* **Models Evaluated:** Random Forest Classification (`ranger`) and Binomial Logistic Regression (`glm`)
* **Analytical Techniques:** K-Means Clustering, RFM Value Modeling, and Geographic Spending Distribution mapping

## 📊 Key Results & Business Value

### 1. Customer Value & Behavioral Modeling
* **RFM Value Engineering:** Grouped transactional data by unique client IDs to model **Recency, Frequency, and Monetary parameters** across 79,916 distinct accounts.
* **Tiered Value Scoring:** Established a standardized 15-point RFM score mapping system to filter top-tier premium clients ("Champions") from dormant profiles.
* **K-Means Cluster Profiling:** Standardized and scaled spending behavioral matrices to segment bank clients into 4 actionable operational profiles.



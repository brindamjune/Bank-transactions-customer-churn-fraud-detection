# Bank Transaction Churn Prediction & Risk Analytics

## 📌 Business Overview
Customer churn and fraud detection are critical challenges in the financial services sector. This project builds an end-to-end predictive and exploratory data analytics pipeline using a dataset of **550,000 retail banking transactions (2019-2024)**. By processing transactional features like transaction hours, credit scores, and account types, this project enables financial institutions to segment customers, perform **RFM (Recency, Frequency, Monetary) value modeling**, and deploy proactive retention strategies before churn occurs.

## 🌟 Key Features

* **End-to-End Data Pipeline:** Cleaned and processed a high-volume transactional dataset containing over **550,000 observations** using the R `tidyverse` ecosystem.
* **RFM Value Engineering:** Transitioned raw timestamp data into actionable **Recency, Frequency, and Monetary (RFM) scores** for 79,916 unique customer profiles, establishing an institutional value hierarchy.
* **Customer Behavioral Segmentation:** Scaled and modeled spending variables using the **K-Means Clustering algorithm** to segment the bank's user base into 4 distinct, targetable client archetypes.
* **Class Imbalance Optimization (`SMOTE`):** Addressed a severe real-world data skew (**only 0.89% of transactions were flagged as fraud**) by implementing Synthetic Minority Over-sampling via the `themis` library to prevent predictive model bias.
* **Predictive Churn Risk Analytics:** Implemented and compared Random Forest Classification (`ranger`) and Binomial Logistic Regression (`glm`) within the `tidymodels` framework to map out the odds ratios of account closures.
* **Geographic Value Mapping:** Aggregated local operational volumes across Indian states to identify and isolate regional spending concentrations.


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

### 2. Risk Mitigation & Fraud Prediction
* **Class Imbalance Optimization:** Handled a severe baseline class imbalance (**only 0.89% of historical cases flagged as fraud**) using Synthetic Minority Over-sampling (`SMOTE`).
* **Risk Driver Analytics:** Executed a Binomial Logistic Regression model to identify features driving customer risk profiles.
* **Statistically Significant Findings:** Uncovered high-confidence feature values (p < 2e-16) demonstrating strong predictive correlations across distinct product account types.

## 🗂️ Project Structure
* `indian_banking_transactions.csv`: Raw data covering bank transaction timelines, credit profiles, loan status flags, and transaction modes.
* `Banking_transactions_churn.ipynb`: Comprehensive notebook executing data preprocessing, exploratory boxplots, value clustering matrices, and random forest validation.

## 🚀 How to Run the Project
1. **Clone the Repository:**
   ```bash
   git clone https://github.com
   ```
2. **Download the Dataset:**
   Download the transaction history from [Kaggle Dataset Hub]([https://kaggle.com](https://www.kaggle.com/datasets/brindamjune/indian-banking-transactions-2019-to-2024)) and place the source file in your designated input directory.
3. **Execute the Pipeline:**
   Open the development environment, install the required packages (`tidymodels`, `themis`, `tidyverse`), and run `Banking_transactions_churn.ipynb`.


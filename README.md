Fraud Detection in E-Commerce Transactions

Project Overview

Online retailers lose billions of dollars each year to fraudulent transactions. Detecting fraud quickly is essential to reducing chargebacks, protecting customers, and minimizing financial risk.

In this project, I analyzed over 1.4 million e-commerce transactions to identify patterns associated with fraudulent activity and built a machine learning model capable of detecting potentially fraudulent transactions.

The project combines:

* Data cleaning
* Exploratory data analysis (EDA)
* Feature engineering
* Fraud risk analysis
* Machine learning classification
* Business recommendations

⸻

BUSINESS QUESTION

Which transaction characteristics are most strongly associated with fraud, and how accurately can machine learning identify fraudulent transactions?

⸻

DATASET

Source:

Fraudulent E-Commerce Transactions Dataset (Kaggle)￼

The dataset contains approximately 1.4 million e-commerce transactions across multiple payment methods, product categories, customer demographics, and device types.

KEY VARIABLES


### Dataset Variables

### Dataset Variables

| Variable | Type | Description |

|-----------|--------|------------|

| Transaction Amount | Numeric | Value of the purchase |

| Transaction Date | Date | Date transaction occurred |

| Payment Method | Categorical | Method used for payment |

| Product Category | Categorical | Product purchased |

| Customer Age | Numeric | Age of customer |

| Device Used | Categorical | Device used for transaction |

| Account Age Days | Numeric | Age of customer account |

| Transaction Hour | Numeric | Hour of transaction |

| Is Fraudulent | Binary | 1 = Fraud, 0 = Legitimate |

---

## Project Workflow

| Stage | Objective | Key Activities | Deliverable |
|---------|------------|---------------|-------------|
| 1. Data Collection | Assemble the transaction dataset | Load and combine two transaction files | Unified dataset containing 1.4 million transactions |
| 2. Data Cleaning | Improve data quality | Check missing values, validate ages, inspect outliers, verify data types | Clean analytical dataset |
| 3. Exploratory Data Analysis (EDA) | Understand fraud patterns | Analyze fraud rates, transaction values, devices, payment methods, account ages, and customer demographics | Visual insights and fraud patterns |
| 4. Feature Engineering | Create predictive variables | Generate account age groups, time-based features, and encoded categorical variables | Enhanced modeling dataset |
| 5. Model Development | Predict fraudulent transactions | Train and evaluate a Random Forest classifier | Fraud prediction model |
| 6. Model Evaluation | Assess model performance | Measure Precision, Recall, F1 Score, and Confusion Matrix | Performance metrics |
| 7. Business Insights | Translate findings into actions | Identify high-risk customer and transaction characteristics | Actionable fraud prevention recommendations |
| 8. Reporting & Visualization | Communicate results | Create charts, dashboard visuals, and project documentation | GitHub portfolio project and dashboard |

## Data Cleaning

| Task | Purpose | Outcome |
|--------|----------|----------|
| Combined transaction files | Create a single dataset for analysis | Unified dataset containing 1.4 million transactions |
| Checked missing values | Identify incomplete records | Assessed data completeness |
| Validated data types | Ensure correct variable formats | Numeric, categorical, and date fields standardized |
| Investigated customer age values | Identify unrealistic ages and outliers | Invalid ages removed or flagged |
| Examined transaction amounts | Detect unusual values and potential anomalies | Distribution reviewed for outliers |
| Converted transaction dates | Enable time-based analysis | Date features created for modeling |
| Checked duplicate records | Prevent double-counting transactions | Duplicate transactions identified and handled |

## Expected Analysis Areas

| Analysis Area | What This Will Investigate |
|--------------|----------------------------|
| Fraud Distribution | How common fraudulent transactions are compared with legitimate transactions |
| Transaction Amount | Whether fraud is associated with higher or lower purchase values |
| Payment Method | Whether certain payment methods show higher fraud exposure |
| Product Category | Which product categories are more vulnerable to fraudulent activity |
| Device Used | Whether fraud differs across mobile, desktop, and tablet transactions |
| Customer Age | Whether age patterns reveal unusual or suspicious behaviour |
| Account Age | Whether newer accounts are more likely to be linked to fraud |
| Transaction Hour | Whether fraud is concentrated at specific times of day |

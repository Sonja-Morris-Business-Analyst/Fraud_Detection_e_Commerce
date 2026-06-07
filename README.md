**Fraud Detection in E-Commerce Transactions**

**PROJECT OVERVIEW**

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

**BUSINESS QUESTION**

Which transaction characteristics are most strongly associated with fraud, and how accurately can machine learning identify fraudulent transactions?

⸻

**DATASET**

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

Exploratory Data Analysis (EDA)
The exploratory analysis investigates patterns and relationships within the transaction data to identify characteristics commonly associated with fraudulent activity.
The analysis focuses on:
Fraud distribution
Transaction amounts
Payment methods
Product categories
Device types
Customer demographics
Account age
Transaction timing
Visualizations
The following visualizations were created during the analysis:
Fraud vs Legitimate Transaction Distribution
Fraud Rate by Payment Method
Fraud Rate by Product Category
Fraud Rate by Device Type
Fraud Rate by Customer Age Group
Fraud Rate by Account Age Group
Fraud Rate by Transaction Hour
Transaction Amount Distribution
Correlation Analysis
Feature Engineering
To improve model performance, additional features were created from the original dataset.
Feature	Purpose
Day of Week	Identify weekly fraud patterns
Month	Identify seasonal trends
Weekend Indicator	Detect behavioural differences between weekdays and weekends
Account Age Group	Categorize customer account maturity
Encoded Categorical Variables	Prepare data for machine learning algorithms
These engineered features were incorporated into the final modeling dataset.
Machine Learning Model
The objective of the machine learning phase was to predict whether a transaction was fraudulent based on transaction characteristics and customer behaviour.
Model Selected
Random Forest Classifier
Random Forest was selected because it:
Handles large datasets efficiently
Works well with mixed feature types
Captures non-linear relationships
Provides feature importance metrics
Is resistant to overfitting
Model Workflow
Step	Description
Data Split	Training and testing datasets created
Feature Encoding	Categorical variables converted into numerical format
Model Training	Random Forest model trained on historical transactions
Prediction	Fraud predictions generated on unseen data
Evaluation	Performance assessed using classification metrics
Model Evaluation
Because fraud datasets are typically highly imbalanced, accuracy alone is not a reliable performance measure.
The model was evaluated using:
Metric	Purpose
Accuracy	Overall prediction performance
Precision	Percentage of predicted fraud cases that were actually fraud
Recall	Percentage of actual fraud cases correctly identified
F1 Score	Balance between precision and recall
Confusion Matrix	Detailed classification performance
Model Results
Metric	Result
Accuracy	To be completed
Precision	To be completed
Recall	To be completed
F1 Score	To be completed
Feature Importance Analysis
Feature importance analysis was used to determine which variables contributed most strongly to fraud prediction.
The analysis helps answer:
Which customer characteristics increase fraud risk?
Which transaction characteristics are most predictive?
Which variables should be monitored in production environments?
Top Predictive Features
To be completed after model training.

BUSINESS RECOMMENDATIONS

Based on the findings, organizations can strengthen fraud prevention efforts through a risk-based monitoring approach.
Potential recommendations include:

Recommendation	Business Benefit
Additional verification for new accounts	Reduce account takeover and synthetic identity fraud
Enhanced monitoring of high-value transactions	Reduce financial losses
Time-based fraud alerts	Detect suspicious activity during high-risk periods
Device and payment method risk scoring	Improve fraud detection accuracy
Continuous model retraining	Adapt to evolving fraud behaviour

Technologies Used
Technology	Purpose
Python	Data analysis and machine learning
Pandas	Data cleaning and transformation
NumPy	Numerical computation
Matplotlib	Data visualization
Seaborn	Exploratory analysis
Scikit-Learn	Machine learning
Google Colab	Development environment
GitHub	Version control and project documentation
Repository Structure
fraud-detection-ecommerce/

├── README.md
├── Fraud_Detection_Analysis.ipynb
├── data/
│   ├── Fraudulent_E-Commerce_Transaction_Data.csv
│   └── Fraudulent_E-Commerce_Transaction_Data_2.csv
├── images/
│   ├── fraud_distribution.png
│   ├── payment_method_fraud.png
│   ├── transaction_hour_fraud.png
│   ├── feature_importance.png
│   └── confusion_matrix.png
└── requirements.txt

*Future Improvements
Potential future enhancements include:
XGBoost implementation
Hyperparameter optimization
Real-time fraud scoring
Interactive Power BI dashboard
Automated fraud monitoring pipeline
Streamlit deployment
Author
Sonja Morris
Data Analytics student with a background in education, business communication, and data-driven problem solving.
Areas of Interest
Fraud Analytics
Business Intelligence
Data Visualization
Predictive Analytics
Data Storytelling

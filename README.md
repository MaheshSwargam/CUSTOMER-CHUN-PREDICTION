# Customer-churn-prediction-codec
Customer Churn Prediction
Analyze customer churn in a sample telecom dataset, explore customer records, and estimate churn risk with a machine-learning model.

Interactive Dashboard
The Streamlit dashboard is the main way to use the project. It provides:

An overview of customer counts, churn rate, and model metrics
A customer table filterable by churn status and account tenure
A form that estimates churn probability from an entered customer profile
Requirements
Python 3.10 or newer
PowerShell on Windows, or a terminal on macOS/Linux
Data
The app reads customer_churn.csv from the project directory. The dataset includes a Churn target column and these customer features:

Feature	Meaning
AccountWeeks	Account tenure in weeks
ContractRenewal	Whether the customer renewed their contract (1 = yes)
DataPlan	Whether the customer has a data plan (1 = yes)
DataUsage	Data usage
CustServCalls	Customer service calls
DayMins	Daytime minutes used
DayCalls	Number of daytime calls
MonthlyCharge	Monthly charge
OverageFee	Overage fee
RoamMins	Roaming minutes
The dashboard trains a random forest classifier from this dataset when it starts. Reported metrics use a held-out test split. Risk scores are model estimates based on this sample data, not guarantees. For real-world use, validate the model with representative, current customer data.

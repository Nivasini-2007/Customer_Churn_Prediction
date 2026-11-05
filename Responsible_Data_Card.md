# Responsible Data Card – Customer Churn Prediction

### 1. Dataset Purpose
The dataset is used to predict whether a customer is likely to leave a service or continue using it. It supports customer retention analysis and helps businesses identify customers who may need additional support. It should not be used to automatically reject customers or make unfair decisions.

### 2. Provenance and Permission
The dataset is provided as a CSV file for this machine learning project. Its original source and licensing permissions should be verified before public or commercial use. Customer information should be handled securely and responsibly.

### 3. Population and Representation
The dataset contains 12 customer records with different subscription plans, spending amounts, support tickets, and login activities. Since the dataset is very small, it may not represent all types of customers. A larger and more diverse dataset is required for reliable predictions.

### 4. Features and Target
The dataset contains the following features:
- Customer ID – Unique customer identification.
- Tenure Months – Number of months the customer has used the service.
- Support Tickets – Number of support requests.
- Monthly Spend INR – Monthly customer spending.
- Last Login Days – Days since the customer's last login.
- Plan Type – Customer subscription category.
- Churned – Target variable (0 = Stayed, 1 = Left).

Customer ID is an identifier and should not be used as a predictive feature.

### 5. Quality Checks
The dataset should be checked for missing values, duplicate records, incorrect values, and outliers. The distribution of churn and non-churn customers should also be examined. Training and testing data should be separated to avoid data leakage.

### 6. Risks and Safeguards
- Bias: Predictions may be inaccurate for underrepresented customer groups.
- Privacy: Customer information must be protected.
- Misuse: Predictions should not be used to unfairly treat customers.
- False Positives: Customers may be incorrectly identified as likely to leave.
- False Negatives: Customers who may leave could be missed.

Human review and regular model evaluation can help reduce these risks.

### 7. Intended Evaluation
The model should be evaluated using accuracy, precision, recall, F1-score, and confusion matrix. Logistic Regression is used as the classification algorithm. Its performance should be compared with a simple baseline model. Fairness, prediction errors, and reliability should also be considered before real-world use.

### Conclusion
This Responsible Data Card explains the purpose, features, limitations, quality requirements, and ethical considerations of the Customer Churn Prediction project. The model is intended for educational purposes and requires further testing with a larger dataset before real-world deployment.

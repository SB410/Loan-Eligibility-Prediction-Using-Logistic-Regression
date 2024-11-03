# Loan-Eligibility-Prediction-Using-Logistic-Regression
This project focuses on building a predictive model to assess whether an applicant is eligible for a home loan based on various factors such as credit history, income, and education. By leveraging data science and machine learning techniques, the model aims to streamline the loan approval process, making it more efficient and objective.

Project Overview

Housing loans are crucial for enabling investments in real estate, but assessing loan eligibility has traditionally been a manual and subjective process. This project employs logistic regression to automate and improve the decision-making process, using historical loan data to train and evaluate the model.

Research Question

Can a data-driven approach accurately predict the eligibility of an individual for a home loan based on a set of relevant features?

Data Summary

	•	Data Source: Kaggle Loan Eligibility Dataset
	•	Number of Observations: 614
	•	Key Variables:
	•	Loan_ID: Unique identifier for each loan
	•	Gender: Male/Female
	•	Married: Applicant married (Yes/No)
	•	Dependents: Number of dependents
	•	Education: Graduate/Undergraduate
	•	Self_Employed: Self-employed (Yes/No)
	•	ApplicantIncome: Income of the applicant
	•	CoapplicantIncome: Income of the co-applicant
	•	LoanAmount: Amount of loan in thousands
	•	Loan_Amount_Term: Term of the loan in months
	•	Credit_History: Credit history meets guidelines (1/0)
	•	Property_Area: Urban/Semi-Urban/Rural
	•	Loan_Status: Loan approved (Yes/No)

Methodology

	1.	Data Cleaning:
	•	Checked and handled missing values using mean or mode imputation.
	•	Performed One-Hot Encoding for categorical variables.
	2.	Feature Selection:
	•	Selected key variables like Credit_History, Education, ApplicantIncome, and Gender.
	3.	Modeling:
	•	Used Logistic Regression for binary classification, with Loan_Status as the target variable.
	•	Conducted multiple iterations to optimize model performance.
	4.	Evaluation:
	•	Measured model accuracy using metrics like precision, recall, F1-score, and confusion matrix.

Results

Logistic Regression Model Performance

	•	Model Accuracy:
	•	Training Data: 80.4%
	•	Testing Data: 82.5%
	•	Confusion Matrix:
	•	True Positives: 68
	•	True Negatives: 17
	•	False Positives: 15
	•	False Negatives: 3
	•	Key Insights:
	•	Credit_History was the most significant predictor of loan eligibility.
	•	The model showed high recall for class ‘1’ (loan approval) but had a lower performance for class ‘0’ (loan rejection).

Limitations

	•	Linear Assumptions: The logistic regression model may not capture complex, non-linear relationships.
	•	Sample Size: Limited sample size may affect model stability and increase the risk of overfitting.
	•	Handling Missing Data: The model is sensitive to missing data, requiring complete datasets for accurate predictions.
	•	Outlier Sensitivity: The model’s performance can be impacted by outliers.

Future Work

	•	Model Improvement: Explore alternative models like Decision Trees, Support Vector Machines (SVM), or ensemble methods for better performance.
	•	Feature Engineering: Investigate additional features or different data transformations to improve model accuracy.
	•	Application Expansion: Extend the model to other loan types, such as auto loans or student loans, with appropriate adjustments to the feature set.

Conclusion

The logistic regression model successfully predicts home loan eligibility with a reasonable accuracy rate. However, there is room for improvement, especially in predicting loan rejections. Further exploration of advanced models and techniques is recommended for enhanced performance.

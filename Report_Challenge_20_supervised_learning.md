# Module 20 Report Template

### Overview of the Analysis###

	##Purpose of the Analysis##

	The purpose of this analysis was to develop machine learning models to predict loan status based 
	on financial information provided in the dataset. Specifically, we aimed to predict whether a loan is
	a healthy loan (0) or a high-risk loan (1) based on features such as loan size, interest rate, borrower 
	income, debt-to-income ratio, number of accounts, derogatory marks, and total debt.

	##Financial Information and Prediction Target##

	The dataset contained financial information related to loans, including loan size, interest rate, 
	borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and 
	loan status (0 for healthy loan, 1 for high-risk loan).

	##Variables to Predict###

	The variable we aimed to predict was the loan status, which had two categories: 0 (healthy loan) and 1 (high-risk loan). 

	Here's the count of each category:

	Healthy loan (0): 18,765 instances
	High-risk loan (1): 619 instances

	##Stages of Machine Learning Process##

	The stages of the machine learning process included:

	Data Loading and Preprocessing: We loaded the dataset, performed basic preprocessing tasks 
	such as handling missing values and encoding categorical variables, and split the data into training and testing sets.

	Model Training: We trained logistic regression models using both the original and resampled training data.

	Model Evaluation: We evaluated the performance of the models using metrics such as accuracy 
	score, balanced accuracy score, precision, recall, F1-score, confusion matrix, and classification report.

	##Methods Used##

	Logistic Regression: We used logistic regression as our classification algorithm to predict loan status based on the given features.
	RandomOverSampler: We used RandomOverSampler to address class imbalance by oversampling the minority class (high-risk loans).


###RESULTS####

Machine Learning Model 1: Logistic Regression on Original Data
Accuracy: 0.99
Precision:
Healthy Loan (0): 1.00
High-Risk Loan (1): 0.85
Recall:
Healthy Loan (0): 0.99
High-Risk Loan (1): 0.91
F1-score:
Healthy Loan (0): 1.00
High-Risk Loan (1): 0.88
These metrics indicate that Machine Learning Model 1 performed very well overall. It achieved high precision, recall, and F1-score values for both healthy and high-risk loans. 

Specifically, the model demonstrated:

Perfect precision (1.00) for predicting healthy loans, indicating that all positive predictions for healthy loans were correct.
High precision (0.85) for predicting high-risk loans, indicating that 85% of the positive predictions for high-risk loans were correct.
High recall for both healthy (0.99) and high-risk (0.91) loans, indicating that the model correctly identified a high proportion of actual instances for both classes.
High F1-score for healthy loans (1.00) and moderately high F1-score for high-risk loans (0.88), indicating a good balance between precision and recall for both classes.

Overall, Machine Learning Model 1 demonstrates strong predictive performance for both healthy and high-risk loans based on the provided evaluation metrics.



Machine Learning Model 2: Logistic Regression on Resampled Data
Accuracy: 0.99
Precision:
Healthy Loan (0): 1.00
High-Risk Loan (1): 0.84
Recall:
Healthy Loan (0): 0.99
High-Risk Loan (1): 0.99
F1-score:
Healthy Loan (0): 1.00
High-Risk Loan (1): 0.91
These metrics indicate that Machine Learning Model 2 performed very well overall. It achieved high precision, recall, and F1-score values for both healthy and high-risk loans. 

Specifically, the model demonstrated:

Perfect precision (1.00) for predicting healthy loans, indicating that all positive predictions for healthy loans were correct.
Moderate precision (0.84) for predicting high-risk loans, indicating that 84% of the positive predictions for high-risk loans were correct.
High recall for both healthy (0.99) and high-risk (0.99) loans, indicating that the model correctly identified a high proportion of actual instances for both classes.
High F1-score for healthy loans (1.00) and moderately high F1-score for high-risk loans (0.91), indicating a good balance between precision and recall for both classes.

Overall, Machine Learning Model 2 demonstrates strong predictive performance for both healthy and high-risk loans based on the provided evaluation metrics.


###Summary####


Both models demonstrate exceptionally high accuracy, precision, recall, and F1-scores, indicating strong performance. 
However, there are differences between the two models, particularly in the precision for high-risk loans.

Model 2 (Logistic Regression on Resampled Data) appears to perform slightly better than Model 1, especially in terms of precision for high-risk loans. 
This improvement is likely due to the data resampling technique employed, which balanced the class distribution.
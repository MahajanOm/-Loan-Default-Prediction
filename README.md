# -Loan-Default-Prediction
Loan Default Prediction
This project is aimed at predicting whether a loan applicant will default on their loan or not, based on several features such as CIBIL score, loan amount, income, and other factors. We use machine learning models to classify applicants into two categories: default (1) or non-default (0).

Steps Involved
Exploratory Data Analysis (EDA):

The dataset was first analyzed to understand the distribution of features, missing values, class imbalance, and relationships between variables.
Key visualizations like histograms, correlation heatmaps, and class distribution charts were created to explore the data.
Data Preprocessing:

Missing values were handled using appropriate imputation techniques.
Categorical variables were encoded using One-Hot Encoding.
SMOTE (Synthetic Minority Over-sampling Technique) was applied to handle class imbalance in the training dataset.
The features were scaled using StandardScaler to ensure all variables were on a similar scale, improving the performance of many machine learning models.
Modeling:

Three machine learning models were used:
Logistic Regression: A simple linear model for binary classification.
Random Forest: An ensemble method that uses multiple decision trees to make predictions.
XGBoost: A gradient boosting model known for its efficiency and high performance.
These models were trained on the preprocessed dataset, and their performance was evaluated using metrics like accuracy, AUC-ROC, and classification report.
Model Selection:

After evaluating the models, XGBoost was chosen as the best model based on its performance in terms of AUC-ROC and accuracy.
The model was selected for its ability to handle complex relationships in the data and its superior performance compared to the other models.
Prediction:

After selecting the best model, it was used to make predictions on new data. The new data was preprocessed and scaled in the same way as the training data before being passed to the model for prediction.
Models Used
Logistic Regression:

Logistic Regression is a linear model used for binary classification. It provides a probabilistic prediction, which is useful for understanding the likelihood of a loan default.
While this model is simple and interpretable, it did not perform as well as more complex models like Random Forest and XGBoost on this task.
Random Forest:

Random Forest is an ensemble learning method that combines multiple decision trees to make predictions. It is more powerful than logistic regression and can capture non-linear relationships in the data.
It performed better than logistic regression but was still outperformed by XGBoost.
XGBoost (Best Model):

XGBoost is an optimized gradient boosting model that typically performs well on tabular data. It excels at handling complex relationships and outperforms many other machine learning models on structured datasets.
Based on evaluation metrics, XGBoost was selected as the best model due to its superior performance in terms of AUC-ROC and accuracy.

How to Use This Repository
Clone the Repository:

Clone this repository to your local machine using the following command:
bash
Copy code
git clone https://github.com/yourusername/loan-default-prediction.git
Install Dependencies:

Install the required Python libraries:
bash
Copy code
pip install -r requirements.txt
Run the Notebook:

Open the Jupyter notebook loan_default_prediction.ipynb in your environment.
Follow the steps in the notebook to load the dataset, preprocess the data, train models, and make predictions.
Upload New Data:

If you have new data (in CSV format), load it into the notebook and follow the prediction steps to get loan default predictions.

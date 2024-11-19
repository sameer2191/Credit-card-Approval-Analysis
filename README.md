# Credit-card-Approval-Analysis
Loan Approval Prediction using Machine Learning

This project utilizes machine learning techniques to predict loan approval statuses for applicants based on their profile attributes such as income, marital status, credit history, and property area. By leveraging classification algorithms, this solution simplifies the loan approval process for banks, improving efficiency and accuracy.
📜 Table of Contents

    About the Project
    Dataset Description
    Technologies Used
    Implementation Steps
    Results
    How to Run
    Conclusion
    License

📖 About the Project

Loans are an integral part of modern financial systems, enabling individuals to manage educational expenses, purchase assets, or cover unforeseen costs. However, assessing a loan applicant’s eligibility involves analyzing numerous factors, which can be time-consuming and prone to errors.

This project builds a machine learning model to predict whether a loan application should be approved or not, based on key features like:

    Applicant Income
    Marital Status
    Credit History
    Property Area, etc.

📊 Dataset Description

The dataset used contains 13 features:
Feature Name	Description
Loan_ID	Unique loan identifier (dropped for modeling)
Gender	Applicant's gender (Male/Female)
Married	Marital status (Yes/No)
Dependents	Number of dependents
Education	Education level (Graduate/Not Graduate)
Self_Employed	Employment type (Yes/No)
ApplicantIncome	Applicant's income
CoapplicantIncome	Co-applicant's income
LoanAmount	Loan amount (in thousands)
Loan_Amount_Term	Loan term (in months)
Credit_History	History of debt repayment
Property_Area	Property location (Rural/Urban/Semi-Urban)
Loan_Status	Loan approval status (Y/N)
⚙️ Technologies Used

    Programming Language: Python
    Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

🔧 Implementation Steps

    Data Preprocessing:
        Dropped irrelevant columns (Loan_ID).
        Encoded categorical variables using Label Encoding.
        Handled missing values by filling them with column means.

    Data Visualization:
        Visualized categorical variables using bar plots.
        Examined correlations between features using a heatmap.
        Explored relationships using catplots.

    Data Splitting:
        Split the data into training and testing sets (60% training, 40% testing).

    Model Training and Evaluation:
        Used multiple classification algorithms:
            Random Forest Classifier
            K-Nearest Neighbors
            Support Vector Machine
            Logistic Regression
        Evaluated models using accuracy scores.

    Model Selection:
        Selected the best-performing model based on accuracy scores on the test set.

📈 Results

    Accuracy Scores on Test Set:
    Model	Accuracy (%)
    Random Forest Classifier	82.50
    Logistic Regression	80.83
    K-Nearest Neighbors	63.75
    Support Vector Machine	69.17

    Best Model: Random Forest Classifier with 82.5% accuracy.

🚀 How to Run

    Clone the repository:

git clone https://github.com/your-username/loan-approval-prediction.git
cd loan-approval-prediction

Install dependencies:

pip install -r requirements.txt

Run the script:

    python main.py

    Modify the dataset file (LoanApprovalPrediction.csv) to test custom inputs.

📌 Conclusion

The Random Forest Classifier achieved the highest accuracy (82.5%) on the test set, making it the most effective model for this loan approval prediction task. Future enhancements could include:

    Implementing ensemble methods like Bagging and Boosting.
    Experimenting with hyperparameter tuning for further optimization.

📄 License

This project is licensed under the MIT License. See the LICENSE file for details.
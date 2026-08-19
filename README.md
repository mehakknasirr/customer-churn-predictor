📊 Telco Customer Churn Prediction
An end-to-end Machine Learning project and web application designed to predict customer churn for telecommunications companies. This project processes customer demographics, services, and billing attributes to identify churn risks and support business retention strategies.

📌 Problem Statement
Customer retention is a primary driver of long-term profitability for subscription-based businesses. Identifying high-risk customers before they cancel services allows marketing and support teams to offer targeted retention incentives, directly reducing revenue loss.

🛠️ Project Architecture & Workflow
 Data Preprocessing: Handled missing values in ⁠TotalCharges⁠ and converted categorical string flags into numeric encodings.
 Feature Pipeline: Standardized numerical variables (⁠tenure⁠, ⁠MonthlyCharges⁠, ⁠TotalCharges⁠) using ⁠StandardScaler⁠ and applied ⁠OneHotEncoder⁠ for categorical inputs.
 
 Model Training: Trained a ⁠RandomForestClassifier⁠ pipeline using ⁠scikit-learn⁠ to classify customer churn likelihood.
 Deployment: Integrated model artifacts via ⁠joblib⁠ into a real-time ⁠Streamlit⁠ interactive application hosted on Streamlit Cloud.
 
📊 Results & Performance
 Model: Random Forest Classifier
 Evaluation Metrics: Evaluated on accuracy and ROC-AUC score to ensure balanced prediction capability across both churned and retained customer classes.
 
🚀 How to Run Locally

1. Clone the Repository

git clone https://github.com/mehakknasirr/customer-churn-predictor.git
cd customer-churn-predictor

3. Install Dependencies
   
pip install -r requirements.txt

5. Run the Streamlit App
   
streamlit run app.py

📁 Repository Structure
├── app.py                         # Streamlit Web Application Interface
├── churn_pipeline_model.pkl       # Trained Model Pipeline Artifact
├── Customer_Churn_Prediction.ipynb # End-to-End Data Science Notebook
├── requirements.txt               # Application Dependencies
└── README.md                      # Documentation

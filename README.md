***💳 Credit Risk Modeling & Scorecard System (FinTech)***

**📌 Overview**

This project builds an end-to-end Credit Risk Modeling system for a fintech/NBFC use case. It predicts the probability of loan default and generates a credit score (300–900) similar to CIBIL, enabling data-driven lending decisions.
The system is deployed using a Streamlit web application, allowing real-time risk assessment based on borrower details.

**🎯 Problem Statement**

Traditional loan approval processes are:

- Manual and time-consuming
- Prone to human bias
- Inefficient in identifying high-risk applicants

This project solves these challenges by building an automated, interpretable ML-based credit scoring system.

**🧠 Solution Approach**

The pipeline follows a real-world fintech workflow:

- Data preprocessing and feature engineering
- Model training using historical loan and default data
- Probability prediction (default risk)
- Conversion of probability → credit score (300–900)
- Risk categorization (Poor → Excellent)
- Deployment via Streamlit UI
  
**⚙️ Tech Stack**

Python
Pandas, NumPy
Scikit-learn
Streamlit
Joblib


**📊 Features Used**

- Demographic Features
- Age
- Financial Features
-  Income
- Loan Amount
- Loan Tenure
- Behavioral Features
- Delinquency Ratio
- Average Days Past Due (DPD)
- Credit Features
- Credit Utilization Ratio
- Number of Open Accounts
- Derived Features
- Loan-to-Income Ratio
  
**🤖 Model Details**

- Algorithm: Logistic Regression
- Feature Scaling: MinMaxScaler
- Model Output: Probability of default

The model is designed to be:

- Interpretable
- Suitable for financial decision-making
- Easy to convert into a scorecard system
- 📈 Credit Score Logic
- Default probability → converted into score range 300–900
- Higher score = lower risk
- 
Risk Categories:
300–500 → Poor
500–650 → Average
650–750 → Good
750–900 → Excellent

**🖥️ Web Application (Streamlit)**

The project includes an interactive UI where users can:

- Input borrower details
- View default probability
- Get credit score
- See risk category instantly
  
**🚀 How to Run Locally**

# Clone repository
git clone https://github.com/<your-username>/credit-risk-scorecard-fintech.git

# Navigate to project folder
cd credit-risk-scorecard-fintech

# Install dependencies
pip install -r requirements.txt

# Run the app
streamlit run app.py

## 📁 Project Structure

```
credit-risk-scorecard-fintech/
│
├── app.py
├── prediction_helper.py
├── requirements.txt
├── README.md
│
├── artifacts/
│   └── model_data.joblib
│
├── notebooks/
│   ├── model_building.ipynb
│   └── ks_analysis.ipynb
│
├── data/
│   └── sample_data.csv
│
├── images/
│   └── ui_screenshot.png
│
└── .gitignore
```

**💡 Business Impact**

- Enables automated loan approval decisions
- Reduces manual underwriting effort
- Improves risk segmentation
- Supports scalable fintech operations
  
**🔮 Future Improvements**

- Add SHAP explainability for model transparency
- Implement ROC-AUC and KS metrics reporting
- Upgrade model to XGBoost / LightGBM
- Deploy as an API (FastAPI)
- Add model monitoring and drift detection
  
**📌 Key Highlights**

- End-to-end ML pipeline (data → model → deployment)
- Real-world fintech use case
- Scorecard-based system (industry relevant)
- Interactive deployment using Streamlit

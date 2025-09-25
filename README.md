Churn Prediction System

📌 Overview

Customer churn is a major challenge for businesses, as retaining existing customers is more cost-effective than acquiring new ones.
This project is a machine learning-based churn prediction system with an interactive web interface built using Streamlit.
It predicts the likelihood of a customer leaving a service and provides clear visual insights to support decision-making.

✨ Features
1. Train and evaluate multiple ML models (Logistic Regression, Random Forest, SVM).
2 Upload datasets in CSV format for analysis.
3. Real-time churn prediction for new customer data.
4. Interactive dashboards with charts:
    - Confusion Matrix
    - ROC Curve
    - Precision-Recall Curve
    - Churn Probability Donut Chart
    - Customer Behavior Bar Charts
5. Simple, user-friendly interface accessible through a web browser.
6. No backend required – runs entirely on client-side.

🏗 Project Structure
```
churn_prediction/
│── Dashboard.py          # Main Streamlit application
│── test.py               # Test script for model evaluation
│── styles.css            # Custom UI styling
│── requirements.txt      # Python dependencies (create this if missing)
│── data/                 # Place your dataset here
```

⚙️ Installation

1. Clone this repository:
```
git clone <repo-url>
cd churn_prediction
```

2. Create and activate a virtual environment (recommended):
```
python -m venv venv
source venv/bin/activate   # On Mac/Linux
venv\Scripts\activate      # On Windows
```

3. Install required dependencies:
```
pip install -r requirements.txt
```

If requirements.txt is missing, install manually:
```
pip install streamlit pandas numpy scikit-learn matplotlib seaborn plotly
```


🚀 Usage
Run the Streamlit app:
```
streamlit run Dashboard.py
```
Upload a dataset (CSV format) with a Churn column.
View predictions, probability scores, and visual insights in the dashboard.


📊 Example Dataset
The system works best with structured datasets containing:
- Demographics (age, gender, region, etc.)
- Service usage (tenure, monthly charges, contract type)
- Churn label (Yes/No)

For testing, you can use the *Telco Customer Churn Dataset*.


🧪 Models Implemented
- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)

Each model is evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC Curve


📈 Results
- Gradient Boosting and Random Forest achieved the highest accuracy in testing.
- The system provides actionable insights for customer retention strategies.


🔒 Security and Privacy
- Runs locally on the client-side.
- No data is stored or transmitted to external servers.
- Safe to use with sensitive datasets.


📌 Future Enhancements
- Integration with CRM systems
- Automated retention strategy suggestions
- Real-time deployment on cloud
= Advanced deep learning models for higher accuracy

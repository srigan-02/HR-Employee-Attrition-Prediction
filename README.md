HR Employee Attrition Prediction – Capstone Project
📌 Project Overview

This project analyzes employee data from Salifort Motors’ HR department to predict whether employees are likely to leave the company. By applying data-driven approaches, the project helps HR identify risk factors contributing to employee attrition and provides actionable insights to improve retention strategies.

The project follows the PACE methodology (Plan, Analyze, Construct, Execute) and uses machine learning models to predict attrition.

🎯 Objectives

Analyze employee satisfaction, workload, salary, department, and other factors.

Identify key drivers of attrition.

Build and evaluate predictive models to classify employees as stayed (0) or left (1).

Provide HR with data-driven recommendations for retention.

Variable	Description
satisfaction_level	Employee job satisfaction (0–1)
last_evaluation	Last performance review score (0–1)
number_project	Number of projects
average_montly_hours	Average monthly hours worked
time_spend_company	Years at the company
Work_accident	Work accident (0 = No, 1 = Yes)
left	Attrition (0 = Stayed, 1 = Left)
promotion_last_5years	Promoted in last 5 years (0 = No, 1 = Yes)
Department	Employee’s department
salary	Salary level (low, medium, high)

⚙️ Project Workflow
1. Data Preparation & Cleaning

Removed duplicates (≈3000 records)

Renamed columns to snake_case

Handled outliers (especially in tenure)

Verified no missing values

2. Exploratory Data Analysis (EDA)

Attrition rate: ~24% employees left

Key patterns observed:

Low satisfaction → higher attrition

High workload (avg monthly hours > 200) → higher attrition

Mid-tenure employees (2–4 years) more likely to leave

Low salary correlated with attrition

Sales & Support departments showed higher turnover

3. Modeling

Task: Binary Classification

Models tested:

Logistic Regression

Decision Tree

Random Forest (best performing)

Evaluation Metrics: Accuracy, Precision, Recall, F1-Score, ROC-AUC

4. Results

Random Forest performed best:

Accuracy: ~88%

ROC-AUC: ~0.90

Key Features Driving Attrition:

Satisfaction level

Average monthly hours

Number of projects

Salary level

Tenure

📊 Visualizations

Satisfaction vs Attrition (boxplot)

Tenure vs Attrition (countplot)

Salary vs Attrition (barplot)

Department vs Attrition (percentage stacked barplot)

Correlation Heatmap

Scatterplot of workload vs evaluation

✅ Insights & Recommendations

Low Satisfaction is the strongest indicator of attrition – HR should conduct regular surveys and act on feedback.

Workload Balance – employees with >200 hrs/month are at higher risk; workload distribution policies may help.

Salary Adjustments – employees with low salaries leave more often; competitive compensation is critical.

Mid-Tenure Risk – employees in years 2–4 should be engaged with growth and recognition opportunities.

Department Focus – Sales and Support require targeted retention programs.

🔒 Ethical Considerations

Privacy: Employee data is anonymized.

Bias: Models must not discriminate based on salary, department, gender, or age.

Transparency: HR must use predictions to improve retention, not penalize employees.

Fairness: Insights should support employee well-being.

📚 Resources

Scikit-learn Documentation

Pandas Documentation

Seaborn Documentation

Matplotlib Documentation

Kaggle HR Analytics Dataset

🚀 How to Run

Clone the repository:

git clone <repo_url>
cd hr-attrition-capstone


Install dependencies:

pip install -r requirements.txt


Run the notebook:

jupyter notebook HR_Capstone_Project.ipynb

📄 Deliverables

Notebook: Full code with EDA, cleaning, modeling, and evaluation.

Summary Report (1-page): Business insights for HR stakeholders.

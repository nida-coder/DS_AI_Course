# 📘 Week 7: Model Evaluation – Customer Churn Prediction

## 🎯 Objective  
Evaluate a **Logistic Regression** model built on the *Customer Churn Dataset* using key classification metrics and visualizations to assess performance and determine the most relevant evaluation metric for the project.

---

## 🧾 Steps Performed  

### 1. **Data Preparation**
- Loaded dataset: `cleaned customer churn dataset.csv`  
- Applied **one-hot encoding** using `pd.get_dummies()` to handle categorical variables  
- Split dataset into:
  - **Training set:** 80%  
  - **Testing set:** 20%

---

### 2. **Model Training**
A **Logistic Regression** model was trained using the Scikit-learn library.

```python
from sklearn.linear_model import LogisticRegression

model = LogisticRegression(max_iter=1000)
model.fit(X_train, y_train)

3. Model Evaluation

The following metrics were calculated to assess model performance:

Metric	Description	Goal
Accuracy	Overall correctness of the model	High
Precision	Fraction of predicted positives that are correct	High
Recall	Ability to detect actual positive cases	High
F1 Score	Balance between Precision and Recall	High
ROC-AUC	Overall classifier performance	High
4. Visualizations

Confusion Matrix: Displays true and false positives/negatives

ROC Curve: Illustrates the trade-off between True Positive Rate (TPR) and False Positive Rate (FPR)

Both visualizations were created using Matplotlib and Seaborn.

📊 Results (Sample Output)
Metric	Value (Example)
Accuracy	0.87
Precision	0.79
Recall	0.84
F1 Score	0.81
ROC-AUC	0.90
💡 Reflection

Which metric is most important for my project and why?

For a Customer Churn Prediction system, the Recall metric is most important.
It measures how well the model identifies customers who are at risk of churning.
A high recall ensures that fewer customers who might actually leave are missed (i.e., minimizes False Negatives).
This allows the business to take proactive retention measures and reduce customer loss.

🧰 Libraries Used

Pandas – Data manipulation and cleaning

NumPy – Numerical computations

Scikit-learn – Model building and evaluation

Matplotlib / Seaborn – Data visualization

⚙️ How to Run
▶️ Option 1: Jupyter Notebook

Open Jupyter Notebook.

Place both the notebook file and the dataset in the same folder.

Run all cells sequentially using Shift + Enter.

💻 Option 2: Python Script

Save the code as model_evaluation.py.

Ensure the dataset file is in the same directory.

Run the script in terminal or command prompt:

python model_evaluation.py

✍️ Prepared By

Name: Nida Sajjad
Course: Data Science / Machine Learning (Week 7)
Assignment: Model Evaluation
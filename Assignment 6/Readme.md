📘 Week 6: Supervised Learning – Classification
🎯 Objective

To apply Logistic Regression and Random Forest on the Customer Churn Dataset, compare their accuracy, and build a baseline classification model.

🧾 Steps Performed
1. Data Loading

Imported dataset cleaned customer churn dataset.csv.

Checked shape and column names.

2. Data Preprocessing

Encoded all categorical variables using LabelEncoder.

Dropped irrelevant ID columns like CustomerID.

Ensured the target variable Churn was correctly defined.

3. Train/Test Split

Split dataset into:

80% training

20% testing

random_state = 42 for reproducibility.

4. Model Training
a. Logistic Regression

Trained using LogisticRegression(max_iter=1000).

Simple baseline model assuming linear relationships.

b. Random Forest Classifier

Trained using RandomForestClassifier(n_estimators=100, random_state=42).

Ensemble model capturing non-linear relationships.

5. Model Evaluation

Evaluated both models using:

Accuracy Score

Confusion Matrix

Classification Report

6. Comparison
Model	Accuracy	Best Model
Logistic Regression	~X.XXX	
Random Forest	~X.XXX	✅ Random Forest (usually higher)

(Fill in with your actual scores after running code.)

📊 Visualizations

Confusion Matrices for both models plotted side-by-side using Seaborn heatmaps.

Helps visualize True/False predictions.

💡 Insights

Logistic Regression gives a fast, interpretable baseline.

Random Forest typically performs better on churn data due to complex decision boundaries.

Feature engineering and hyperparameter tuning can further improve accuracy.

🧰 Libraries Used

Pandas, NumPy – Data handling

Scikit-Learn – Machine Learning models and metrics

Matplotlib, Seaborn – Visualizations

⚙️ How to Run
🔹 Option 1: Jupyter Notebook

Open Jupyter Notebook or Google Colab.

Upload both:

cleaned customer churn dataset.csv

Notebook file .ipynb

Run each cell in order.

🔹 Option 2: Python Script

Save code as classification_models.py.

Place the dataset in the same directory.

Run in terminal:

python classification_models.py


Check printed accuracy results and confusion matrices.

🚀 Next Steps (Project Milestone)

Perform feature selection to remove weak predictors.

Apply hyperparameter tuning using GridSearchCV.

Experiment with Gradient Boosting or XGBoost for better performance.

Integrate the best model into your E-commerce Recommendation System.
🖋 Prepared By: Nida Sajjad
📅 Week 6 – Classification Assignment
📘 Week 8: Unsupervised Learning – K-Means Clustering + PCA
🎯 Objective

To apply K-Means Clustering on the Customer Churn Dataset and visualize the resulting clusters in 2D using Principal Component Analysis (PCA).
This helps discover hidden customer segments without using labels.

🧾 Steps Performed
1. Data Loading

Loaded the dataset cleaned customer churn dataset.csv using Pandas.

Displayed basic information such as shape and columns.

2. Data Preprocessing

Dropped identifier columns like CustomerID.

Converted categorical columns into numerical form using One-Hot Encoding (pd.get_dummies()).

Standardized the data using StandardScaler to normalize different feature scales.

3. K-Means Clustering

Applied K-Means from Scikit-learn.

Used the Elbow Method to determine an optimal number of clusters (k).

Chose k = 3 for simplicity.

Assigned each customer a Cluster label.

4. PCA for Dimensionality Reduction

Applied Principal Component Analysis (PCA) to reduce all features to 2 dimensions.

This makes cluster visualization easier and interpretable.

5. Visualization

Used Seaborn scatterplot to show clusters in 2D PCA space:

Each color represents a different cluster.

The spread of points shows how distinct the clusters are.

6. Cluster Analysis

Calculated mean values of each feature per cluster to understand group characteristics.

Example:

Cluster 0: Low-spend, high-churn customers

Cluster 1: Loyal, long-tenure customers

Cluster 2: Moderate activity segment

📊 Libraries Used

Pandas – Data loading and cleaning

NumPy – Numerical computations

Scikit-Learn – K-Means, PCA, StandardScaler

Matplotlib & Seaborn – Visualization

⚙️ How to Run
🔹 Option 1: Jupyter Notebook

Open Jupyter Notebook.

Place the .ipynb file and cleaned customer churn dataset.csv in the same directory.

Run each cell in order using:

Shift + Enter


Observe:

Elbow Method plot

2D Cluster visualization

Cluster summary and insights

🔹 Option 2: Python Script

Save the code as unsupervised_clustering.py.

Ensure the dataset is in the same folder.

Run the script from terminal:

python unsupervised_clustering.py


View results and plots in your output window.

💡 Insights

Unsupervised clustering helps identify hidden patterns in customers.

This can guide:

Personalized marketing strategies

Retention campaigns

Product recommendations

PCA enables visual understanding of these clusters in 2D.

🖋 Prepared By: Nida Sajjad
📅 *Week 8 – Unsupervised Learning Assignment
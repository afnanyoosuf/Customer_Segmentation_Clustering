 Customer Segmentation using Unsupervised Learning
 Project Overview

This project performs an end-to-end unsupervised learning workflow on the Mall Customer Segmentation Dataset.
The goal is to segment customers based on their demographics and spending behavior to derive business-ready insights.

The project covers:

Exploratory Data Analysis (EDA)

Feature engineering and preprocessing

K-Means clustering with evaluation (Elbow Method & Silhouette Score)

Cluster visualization (including PCA)

Comparison with Hierarchical Clustering and DBSCAN

Business interpretation of clusters and actionable strategies

Repository Structure
Customer_Segmentation_Clustering/
│
├── data/
│   └── mall_customers.csv        # Dataset
│
├── notebooks/
│   ├── 01_eda.ipynb              # Data understanding & EDA
│   ├── 02_preprocessing.ipynb    # Feature engineering & scaling
│   ├── 03_clustering.ipynb       # K-Means, Hierarchical, DBSCAN, Visualization & Interpretation
│
├── requirements.txt              # Python dependencies
└── README.md                     # Project documentation

How to Run the Project

Clone the repository:

git clone <https://github.com/afnanyoosuf/Customer_Segmentation_Clustering>
cd Customer_Segmentation_Clustering


Install dependencies:

pip install -r requirements.txt


Open Jupyter Notebook:

jupyter notebook


Run notebooks in order:

01_eda.ipynb

02_preprocessing.ipynb

03_clustering.ipynb

Tasks Covered
Task 1: Rapid Data Understanding & EDA

Plots:

Income vs Spending

Age distribution

Gender vs Spending

Additional exploratory plot

Derived multiple insights, including non-obvious patterns in spending vs income.

Task 2: Feature Engineering & Preprocessing

Tried different feature combinations:

(Annual Income, Spending Score)

(Age, Annual Income, Spending Score)

Encoded categorical variables (Gender) where needed.

Applied StandardScaler.

Explained why K-Means is sensitive to scaling (distance-based algorithm).

Task 3: K-Means Deep Dive

Used:

Elbow Method

Silhouette Score

Selected final value of k with justification.

Added cluster labels to the dataset.

Explained:

What happens when k increases or decreases

The trade-off between simplicity and over-segmentation

Task 4: Cluster Visualization & Geometry

Visualized:

Income vs Spending with centroids

PCA projection for multi-dimensional visualization

Explained what visualizations reveal beyond numerical metrics (cluster separation, overlap, geometry).

Task 5: Algorithm Comparison

Applied:

Hierarchical Clustering (Agglomerative)

DBSCAN

Compared algorithms based on:

Strengths

Weaknesses

When to use

Explained why different algorithms produce different clustering results.

Task 6: Cluster Interpretation & Business Strategy

For each clustering method:

Created cluster profiles

Defined customer personas

Proposed actionable business decisions

Included risks and limitations for at least one recommendation

Key Conclusions

K-Means provides clear and actionable customer segments for marketing strategies.

Hierarchical clustering helps understand relationships between segments.

DBSCAN is useful for detecting outliers and unusual customer behavior.

Visualizations (especially PCA) help interpret cluster geometry beyond numerical scores.

Different algorithms serve different business and analytical goals, so choosing the right one depends on the problem context.

Time Spent Per Task (Approximate & Honest)

Task 1: EDA → ~4 hours

Task 2: Preprocessing → ~4 hours

Task 3: K-Means & Evaluation → ~4 hours

Task 4: Visualization → ~2 hour

Task 5: Algorithm Comparison → ~4 hours

Task 6: Business Interpretation → ~2 hours

Requirements

See requirements.txt for full list. Main libraries used:

pandas

numpy

matplotlib

seaborn

scikit-learn

Final Note

This project demonstrates a complete unsupervised learning pipeline from raw data to business insights, following professional structure and GitHub practices.

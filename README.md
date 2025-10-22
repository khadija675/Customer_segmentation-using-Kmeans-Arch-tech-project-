# Customer_segmentation-using-Kmeans-Arch-tech-project-
# 🛍️ Mall Customer Segmentation using K-Means Clustering

## Project Overview

This project focuses on performing **customer segmentation** using the **K-Means Clustering** algorithm on a dataset of mall customers. The goal is to identify distinct groups of customers based on key attributes—specifically **Annual Income** and **Spending Score**—to enable targeted marketing and improved business strategy.

This analysis was completed as part of an internship at [Your Internship Company Name or just 'a data science internship'].

## 🎯 Business Goal

To segment the customer base into meaningful, actionable groups to answer questions like:
* Which customers are high-value targets (High Income & High Spenders)?
* Which customers have high income but low spending (Untapped Potential)?
* How can marketing campaigns be tailored for each segment?

## 🛠️ Tools and Libraries

* **Language:** Python
* **Core Libraries:** Pandas, NumPy
* **Machine Learning:** Scikit-learn (KMeans)
* **Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook / Google Colab

## 📊 Data

The project uses the `Mall_Customers.csv` dataset, which includes 200 customer records with the following attributes:
* `CustomerID`
* `Gender`
* `Age`
* `Annual Income (k$)`
* `Spending Score (1-100)`

**Key Features Used for Clustering:** `Annual Income (k$)` and `Spending Score (1-100)`.

## 💡 Methodology

1.  **Exploratory Data Analysis (EDA):** Analyzed distributions and relationships between `Annual Income` and `Spending Score`.
2.  **Feature Selection:** Extracted the two most relevant features for clustering.
3.  **Optimal Cluster Selection (Elbow Method):** Used the Within-Cluster Sum of Squares (WCSS) plot to determine the most effective number of clusters (**k=5**).
4.  **Model Training:** Applied the **K-Means algorithm** with $k=5$ to segment the customers.
5.  **Visualization:** Plotted the final clusters and their centroids to clearly define each customer group.

## 🔑 Key Findings (Customer Segments)

The K-Means model successfully identified 5 actionable customer segments. This is the most crucial part for showcasing the business value:

| Cluster | Income | Spending Score | Segment Profile | Actionable Strategy |
| :---: | :---: | :---: | :--- | :--- |
| **4** | High | High | **Target Customers (VIPs)** | Focus on loyalty, premium products, and personalized service. |
| **0** | High | Low | **Careful Spenders** | Offer value-added services, bundled deals, or credit incentives to increase spending frequency. |
| **3** | Low | High | **Impulsive Spenders** | Focus on promotional items, budget-friendly offers, and high-turnover products. |
| **1** | Mid | Mid | **Average** | Standard marketing and occasional promotions. |
| **2** | Low | Low | **Frugal** | Minimal marketing or targeted clearance sales. |

## 🚀 How to Run the Project

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/khadija675/Customer_segmentation-using-Kmeans-Arch-tech-project-/edit/main/README.md]
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn
    ```
3.  **Run the analysis:**
    * Open `Customer Segmentation.ipynb` in a Jupyter environment (Jupyter Lab, VS Code, or Google Colab).
    * Execute all cells sequentially to reproduce the analysis and the final cluster visualization.

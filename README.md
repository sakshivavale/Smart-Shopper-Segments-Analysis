# 🛍️ Mall Customer Segmentation using K-Means Clustering

An interactive Machine Learning project that performs customer segmentation using unsupervised learning (**K-Means Clustering**). By analyzing customer demographics, annual income, and spending behaviors, this project identifies targeted customer profiles to help marketing teams optimize customer engagement strategies.

---

## 📌 Project Overview

Customer segmentation is the process of dividing a target market into distinct groups of consumers who share similar characteristics. In this project, we analyze the **Mall Customers** dataset using Python data science libraries to group customers into 5 distinct behavioral clusters.

### Key Objectives:
1. **Data Preprocessing & Feature Scaling:** Standardize features using `StandardScaler` to treat income and spending score metrics equally.
2. **Optimal Cluster Selection:** Identify the ideal number of clusters ($K$) using the **Elbow Method** (WCSS / Inertia).
3. **K-Means Modeling:** Apply `KMeans` clustering algorithm to segment the dataset.
4. **Cluster Profiling:** Calculate aggregated statistics (Average Age, Income, Spending Score, and Group Count) for strategic insights.

---

## 📊 Dataset Overview

The project utilizes `Mall_Customers.csv`, which includes the following features:

| Column Name | Feature Description |
| :--- | :--- |
| `CustomerID` | Unique numerical identifier for each customer |
| `Genre` | Gender of the customer (`Male` / `Female`) |
| `Age` | Age of the customer (years) |
| `Annual Income (k$)` | Annual income of the customer in thousands of dollars |
| `Spending Score (1-100)` | Score assigned by the mall based on customer behavior and spending patterns |

---

## 💡 Cluster Profiles & Business Insights

Based on K-Means clustering ($K=5$), the customer base is segmented into the following groups:

| Cluster Label | Target Persona | Avg Age | Avg Income (\$k) | Avg Spending Score | Strategy Focus |
| :---: | :--- | :---: | :---: | :---: | :--- |
| **0** | **Moderate / Standard** | ~42.7 | ~\$55.3k | ~49.5 | Loyalty & steady engagement |
| **1** | **Target High Value** | ~32.7 | ~\$86.5k | ~82.1 | Premium product offers & VIP events |
| **2** | **Careless / Big Spenders** | ~25.3 | ~\$25.7k | ~79.4 | Budget deals & fast-fashion promotions |
| **3** | **Frugal / High Earners** | ~41.1 | ~\$88.2k | ~17.1 | Exclusive quality & luxury discounts |
| **4** | **Sensible / Low Spenders** | ~45.2 | ~\$26.3k | ~20.9 | Discount vouchers & essentials |

---

## 🛠️ Tech Stack & Libraries

- **Language:** Python 3.x
- **Data Manipulation:** `pandas`, `numpy`
- **Data Visualization:** `matplotlib`, `seaborn`
- **Machine Learning:** `scikit-learn` (`KMeans`, `StandardScaler`)
- **Environment:** Google Colab / Jupyter Notebook

---

## 📁 Project Structure

```text
├── Mall_Customers.csv       # Raw customer dataset
├── Customer_Segmentation.ipynb # Python Google Colab Notebook
├── segmented_customers.csv  # Output dataset with assigned cluster labels
└── README.md                # Project documentation

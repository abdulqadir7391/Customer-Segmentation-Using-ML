# 🧠 Customer Segmentation Analysis

This project analyzes customer behavior using a dataset of 52,000+ customer records and applies machine learning (K-Means clustering) to identify meaningful customer segments for business insights and marketing personalization.

The project includes:

- 🔍 Exploratory Data Analysis (EDA)
- 📊 Visual analysis using Power BI dashboards
- 🤖 Machine Learning–based customer segmentation
- 📁 Clean documentation with reproducible notebook workflow

---

## 📂 Project Structure

Customer-Segmentation-Analysis/
│
├── data/
│ └── customer_data.csv (or customer_data_sample.csv if dataset is large/private)
│
├── notebook/
│ └── analysis.ipynb
│
├── report/
│ └── Customer_Segmentation_Report.pdf
│
└── README.md

## 🚀 Tech Stack

| Component | Tools |
|----------|-------|
| Programming Language | Python |
| Data Processing | Pandas, NumPy |
| Visualization | Power BI, Matplotlib, Seaborn |
| Machine Learning | Scikit-Learn (K-Means Clustering) |
| Notebook | Jupyter Notebook |

---

## 📊 Dashboard Highlights (Power BI)

The Power BI report visualizes:

- 🧑‍🤝‍🧑 Total Customers: **40,259**
- 💰 Total Sales: **₹161.8 Million**
- ⭐ Average Rating: **2.9**
- 📍 Segmentation based on:
  - Gender
  - Language
  - Geography (State)
  - Income Group
  - Marital Status
  - Age Group
  - Education Levels

## 🔍 Data Preprocessing

- Standardized column names (lowercase, snake_case format)
- Handled missing values
- Extracted relevant features for segmentation:

## 🤖 Machine Learning: K-Means Clustering

To determine the optimal number of clusters, the **Silhouette Score Evaluation** was used with values from k=2 to k=9.

### 📈 Silhouette Evaluation Results

| k | Score |
|---|-------|
| 2 | 0.3716 |
| 3 | 0.4132 |
| **4** | **0.4299 (Best)** |
| 5 | 0.3918 |
| 6 | 0.3734 |
| 7 | 0.3889 |
| 8 | 0.3831 |
| 9 | 0.3867 |

👉Based on evaluation, **4 clusters** provided the best structure and separation.

---

## 🧩 Final Customer Segments

| Segment Name | Behavioral Summary | Traits |
|--------------|--------------------|--------|
| **Segment 1: Premium Customers** | High-value, loyal buyers | High income, high total spending, good ratings |
| **Segment 2: Growth Customers** | Mid-tier but promising | Average spending, younger demographic |
| **Segment 3: Budget/Price-Sensitive Customers** | Low spend, irregular purchases | Lower income, lower engagement |
| **Segment 4: At-Risk/Low Activity Customers** | Likely churn category | Low ratings, minimal activity |

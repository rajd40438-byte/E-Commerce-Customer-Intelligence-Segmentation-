# E-Commerce-Customer-Intelligence-Segmentation-
Customer analytics framework combining RFM segmentation, clustering and Customer Lifetime Value modeling
# E-Commerce Customer Intelligence & Segmentation

## 📌 Project Overview

This project develops a customer intelligence framework for an e-commerce business using transaction-level data.

The objective is to transform raw transaction data into actionable customer insights by combining:

* Exploratory Data Analysis
* RFM Analysis
* Customer Segmentation
* K-Means Clustering
* Customer Lifetime Value (CLV) analysis
* Customer prioritization
* Retention strategy recommendations

The project focuses on answering an important business question:

> **Which customers are most valuable, which customers are at risk, and how should marketing efforts be prioritized?**

---

## 🎯 Business Objectives

The analysis aims to:

1. Understand overall e-commerce sales performance.
2. Identify high-value customers.
3. Measure customer recency, frequency and monetary value.
4. Segment customers according to purchasing behavior.
5. Identify potentially high-value customers at risk of becoming inactive.
6. Estimate customer value using CLV techniques.
7. Provide actionable customer retention recommendations.

---

## 📊 Dataset

The project uses transaction-level online retail data containing information such as:

* Invoice number
* Product / Stock Code
* Product description
* Quantity
* Invoice date
* Unit price
* Customer ID
* Country

The dataset is used to construct customer-level behavioral and monetary features.

> **Note:** The original dataset is not included in this repository. Please obtain it from the original dataset source and place it in the appropriate local `data/` directory.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Lifetimes
* Jupyter Notebook

---

## 🔍 Methodology

### 1. Data Preparation

The transaction data is examined for:

* Missing customer identifiers
* Duplicate records
* Invalid quantities
* Invalid prices
* Cancelled transactions
* Date and numeric formatting

Revenue is calculated as:

**Revenue = Quantity × Unit Price**

---

### 2. Exploratory Data Analysis

The project analyzes:

* Total revenue
* Number of customers
* Number of orders
* Number of products
* Average order value
* Monthly revenue trends
* Product performance
* Country-level performance

---

### 3. RFM Analysis

Customers are evaluated using:

| Metric    | Meaning                             |
| --------- | ----------------------------------- |
| Recency   | How recently the customer purchased |
| Frequency | How often the customer purchased    |
| Monetary  | How much the customer spent         |

RFM scores are then used to create interpretable customer segments such as:

* Champions
* Loyal / Active Customers
* New / Potential Customers
* At-Risk Customers
* High-Value At-Risk Customers

---

### 4. K-Means Customer Segmentation

RFM features are transformed and standardized before applying K-Means clustering.

The number of clusters is evaluated using:

* Elbow Method
* Silhouette Score

The final cluster solution is then profiled using customer recency, frequency and monetary behavior.

---

### 5. Customer Lifetime Value

Customer value is analyzed using historical purchasing behavior and CLV modeling techniques.

The analysis is used to identify customers with greater potential business value and support retention prioritization.

---

## 📈 Key Results

The completed analysis covered approximately:

* **4,300+ customers**
* **19,000+ orders**
* **4,000+ products**
* **£8.8M+ historical revenue**

The customer segmentation framework combines RFM-based behavioral interpretation with K-Means clustering.

The final analysis also identifies high-value customers and supports targeted retention strategies.

---

## 💼 Business Insights

The analysis supports differentiated strategies for different customer groups.

### High-Value Customers

Prioritize:

* Loyalty programs
* VIP benefits
* Cross-selling
* Personalized offers

### New / Potential Customers

Focus on:

* Second-purchase incentives
* Onboarding campaigns
* Personalized product recommendations

### At-Risk High-Value Customers

Prioritize:

* Win-back campaigns
* Personalized discounts
* Targeted communication

These customers represent an important retention opportunity because of their historical purchasing value.

### Low-Value / Inactive Customers

Use:

* Automated campaigns
* Low-cost communication
* Limited retention spending

---

## 📁 Repository Structure

```text
├── README.md
├── E-Commerce-Customer-Intelligence.ipynb
├── requirements.txt
├── data/
│   └── README.md
├── outputs/
│   └── customer_intelligence_output.csv
└── .gitignore
```

---

## 🚀 How to Run

Clone the repository:

```bash
git clone https://github.com/rajd40438-byte/E-Commerce-Customer-Intelligence-Segmentation.git
```

Navigate to the project:

```bash
cd E-Commerce-Customer-Intelligence-Segmentation
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Open the notebook:

```bash
jupyter notebook
```

Place the dataset in the appropriate location and update the dataset path in the notebook before running the analysis.

---

## 👤 Author

**RajKumar Das**

GitHub: [rajd40438-byte](https://github.com/rajd40438-byte)

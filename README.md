# final-capstone-project--advanced-python
Final Capstone Project

# Customer & Product Segmentation using K-Means Clustering

## 📌 Project Overview

This capstone project demonstrates how **K-Means Clustering**, an unsupervised machine learning algorithm, can be used to segment customers and products based on purchasing behavior. Using a real-world online retail dataset, the project identifies different customer and product groups to help businesses make data-driven decisions in marketing, customer retention, and inventory management.

The project follows a complete data analytics workflow, including:

- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Feature engineering
- Customer segmentation
- Product segmentation
- Data visualization
- Business recommendations

---

## 🎯 Objectives

- Clean and prepare a real-world retail dataset.
- Explore customer purchasing behavior through data analysis.
- Segment customers based on purchasing patterns.
- Segment products based on sales performance.
- Apply K-Means clustering for unsupervised learning.
- Visualize the resulting clusters.
- Generate business insights and recommendations.

---

## 📂 Dataset

**Dataset:** Online Retail Dataset

This dataset contains one year of transactional data from a UK-based online retail company.

### Features

| Column | Description |
|---------|-------------|
| InvoiceNo | Invoice number |
| StockCode | Product code |
| Description | Product description |
| Quantity | Number of items purchased |
| InvoiceDate | Date and time of purchase |
| UnitPrice | Price per unit |
| CustomerID | Unique customer identifier |
| Country | Customer's country |

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- ydata-profiling
- Jupyter Notebook

---

## 📊 Project Workflow

### 1. Data Cleaning

The dataset was prepared by:

- Filling missing product descriptions using the StockCode.
- Removing records with missing Customer IDs.
- Removing cancelled transactions.
- Removing invalid quantities and unit prices.
- Removing duplicate records.
- Excluding incomplete data from December 2011.
- Converting columns into appropriate data types.

---

### 2. Exploratory Data Analysis (EDA)

EDA was performed using **ydata-profiling** to better understand the dataset, including:

- Missing values
- Summary statistics
- Data distributions
- Feature relationships

---

### 3. Customer Segmentation

Three customer metrics were calculated:

- **Total Sales**
- **Order Count**
- **Average Order Value**

The features were ranked, normalized, and clustered using **K-Means Clustering**.

The optimal number of clusters was determined using the **Silhouette Score**, resulting in **4 customer segments**.

#### Customer Segments

| Segment | Description | Business Strategy |
|----------|-------------|-------------------|
| VIP Customers | High spending and frequent purchases | Loyalty programs, exclusive rewards, premium services |
| Frequent Small Buyers | Purchase frequently but spend less per order | Bundle deals, upselling, minimum-spend promotions |
| Occasional Big Spenders | Spend a lot per order but purchase infrequently | Membership programs, reminders, re-engagement campaigns |
| Low-Value Customers | Low spending and low purchase frequency | Discounts, free shipping, promotional campaigns |

---

### 4. Product Segmentation

Products were segmented using:

- Total Sales
- Total Quantity Sold
- Order Count
- Average Order Quantity

K-Means clustering was then applied to identify four different product groups based on their sales performance.

---

## 📈 Visualizations

### Customer Segmentation

- Total Sales vs Order Count
- Total Sales vs Average Order Value
- Order Count vs Average Order Value

### Product Segmentation

- Order Count vs Average Order Quantity
- Total Sales vs Total Quantity Sold
- Average Order Quantity vs Total Sales

---

## 💡 Key Insights

### Customer Insights

- VIP customers generate the highest revenue and should be retained through loyalty programs and personalized services.
- Frequent buyers with lower spending can be encouraged to increase their basket size through upselling and bundle promotions.
- Customers with high order values but low purchase frequency can be re-engaged using personalized reminders and membership programs.
- Low-value customers can be reactivated through discounts and promotional campaigns.

### Product Insights

- High-performing products contribute significantly to total sales and should remain a business priority.
- Frequently purchased products with lower sales present opportunities for pricing or bundling strategies.
- Low-performing products may benefit from promotional campaigns or inventory optimization.

---

## 📁 Repository Structure

```text
Customer-Segmentation/
│
├── Final Capstone Project.ipynb
├── Online Retail.xlsx
├── order_detail_report.html
├── README.md
└── requirements.txt
```

---

## ▶️ Installation

Clone this repository:

```bash
git clone https://github.com/yourusername/customer-segmentation.git
```

Navigate to the project directory:

```bash
cd customer-segmentation
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib scikit-learn ydata-profiling openpyxl
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

---

## 📚 Learning Outcomes

Through this project, I gained hands-on experience in:

- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Customer Analytics
- Product Analytics
- Unsupervised Machine Learning
- K-Means Clustering
- Silhouette Score Evaluation
- Business Insight Generation
- Data Visualization using Matplotlib

---

## 🚀 Future Improvements

- Compare K-Means with other clustering algorithms such as Hierarchical Clustering and DBSCAN.
- Build an interactive dashboard using Power BI or Tableau.
- Develop a product recommendation system.
- Deploy the project as a Streamlit web application.
- Perform RFM (Recency, Frequency, Monetary) analysis for deeper customer segmentation.

---

## 👩‍💻 Author

**Su Myat Noe**

Student at Python Myanmanr Institute

---

## 📖 Educational Purpose

This repository was developed as part of a school capstone project for educational purposes. The project demonstrates the application of Python, data analytics, and machine learning techniques to solve a real-world business problem through customer and product segmentation.

If you are learning Python, data analytics, or machine learning, feel free to explore the notebook, use the code as a reference, and build upon it for your own learning.

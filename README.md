# 👨🏻‍💻 Customer Behavior Data Analyst Project

This project represents a complete, industry-standard, end-to-end data analytics workflow, designed to mirror the real responsibilities of professional analysts in modern business environments. The project encompasses all critical stages of data analysis, from data preparation and modeling to insight generation, visualization, and reporting.

## 📌 Project Overview

The goal of this project is to simulate a corporate-grade end-to-end data analytics workflow, demonstrating the ability to translate raw data into strategic business intelligence by:

✅ **Data Preparation, Modeling & Exploratory Data Analysis (Python)**: Clean and transform the raw dataset for analysis.

✅ **Data Analysis (SQL)**: Run queries to extract insights on customer segments, loyalty, and purchase drivers.

✅ **Visualization & Insights (Power BI)**: Build an interactive dashboard that highlights key patterns and trends, enabling stakeholders to make data-driven decisions.

✅ **Report and Presentation**: Summarize key findings and business recommendations.

## Business Problem

A retail company wants to better understand customer purchasing behavior to improve customer retention, optimize marketing campaigns, and identify high-value customer segments.

This project analyzes customer demographics, spending patterns, and purchase frequency using SQL, Python, and Power BI to generate actionable business insights.

📄 ./reports/Business_Problem_Document.pdf

## 📊 Dataset

**Source**: Retail Customer Shopping Behavior Dataset  
**Size**: 3,900 transactions × 18 features  
**Features**:
- Customer ID, Age, Gender
- Item Purchased, Category (Clothing, Footwear, Accessories, Outerwear)
- Purchase Amount (USD), Location (US State)
- Size, Color, Season
- Review Rating (1-5), Subscription Status
- Shipping Type, Discount Applied
- Previous Purchases, Payment Method
- Frequency of Purchases

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **Python** (pandas, SQLAlchemy) | Data cleaning, EDA, feature engineering, SQL export |
| **SQL** (PostgreSQL / MySQL / MS SQL Server) | Business question analysis |
| **Power BI** | Interactive dashboard visualization |
| **Jupyter Notebook** | Analysis documentation |

## 📁 Project Structure

```
customer-shopping-behavior-analysis/
├── data/
│   └── customer_shopping_behavior.csv       
├── notebooks/
│   └── Customer_Shopping_Behavior_Analysis.ipynb  
├── sql/
│   └── customer_behavior_sql_queries.sql    
├── dashboard/
│   └── customer_behavior_dashboard.pbix     
├── reports/
│   ├── Business Problem Document.pdf        
│   ├── Customer Shopping Behavior Analysis.pdf  
│   └── Customer-Shopping-Behavior-Analysis.pptx 
├── requirements.txt                          
├── LICENSE                                   
└── README.md                                 
```

## 🚀 How to Run This Project

### 1. Clone & Setup
```bash
git clone <your-github-repo-url>
cd customer-shopping-behavior-analysis
pip install -r requirements.txt
```

### 2. Python Analysis (Jupyter Notebook)
Open `notebooks/Customer_Shopping_Behavior_Analysis.ipynb` in VS Code or JupyterLab:
- Run all cells to perform EDA, cleaning, and feature engineering
- The notebook creates derived columns: `age_group`, `purchase_frequency_days`
- Updates column names to snake_case

### 3. Load Data into SQL Database

**Option A: PostgreSQL**
```sql
CREATE DATABASE customer_behavior;
```
Update credentials in notebook (Cell 19) and run the SQLAlchemy export.

**Option B: MySQL**
```sql
CREATE DATABASE customer_behavior;
```
Update credentials in notebook (Cell 21) and run.

**Option C: MS SQL Server**
- Install Microsoft ODBC Driver 17
- Update credentials in notebook (Cell 23) and run.

### 4. SQL Analysis
Open `sql/customer_behavior_sql_queries.sql` in your SQL client and execute the 10 queries:
1. Revenue by gender
2. Discount users spending above average
3. Top 5 products by review rating
4. Standard vs Express shipping comparison
5. Subscriber vs non-subscriber spending
6. Top 5 products by discount rate
7. Customer segmentation (New/Returning/Loyal)
8. Top 3 products per category
9. Repeat buyers' subscription likelihood
10. Revenue by age group

### 5. Power BI Dashboard
1. Open `dashboard/customer_behavior_dashboard.pbix` in Power BI Desktop
2. Connect to your SQL database (Transform Data → Change Source)
3. Refresh to load your data
4. Explore the interactive dashboard

### 6. Reports & Presentation
- **Business Problem Document**: Project scope and objectives
- **Analysis Report**: Detailed findings and insights
- **Presentation Deck**: Ready-to-present slides (customize with your findings)

## 🔑 Key Insights (From Analysis)

| Insight | Finding |
|---------|---------|
| **Gender Revenue** | Compare male vs female customer revenue contribution |
| **Discount Behavior** | Customers using discounts who still spend above average |
| **Product Ratings** | Top-rated products by category |
| **Shipping Impact** | Express vs Standard shipping average order value |
| **Subscription Value** | Subscribers vs non-subscribers spending patterns |
| **Customer Loyalty** | New/Returning/Loyal segment distribution |
| **Category Leaders** | Top 3 products per category |
| **Age Group Revenue** | Revenue contribution by age segment |

*Run the SQL queries to generate actual numbers for your portfolio.*

## 📈 Dashboard Preview

The Power BI dashboard includes:
- Revenue KPIs by gender, category, season
- Customer segmentation visuals
- Shipping type analysis
- Subscription status comparison
- Geographic distribution (US states)
- Interactive filters and slicers

## 📝 License

MIT License — feel free to fork, star, and use in your portfolio. See [LICENSE](LICENSE) for details.

## 📬 Connect

If you found this project helpful, feel free to connect:
-  ([LinkedIn](https://www.linkedin.com/in/dev-durgesh-shukla/))
-  ([GitHub](https://github.com/beingDurgesh))

---

⭐ **Star this repo if you found it useful!**  
*Built as part of my Data Analytics portfolio to demonstrate end-to-end analysis skills.*
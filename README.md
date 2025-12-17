# Customer Shopping Behavior Analysis

## 📌 Project Overview

This project analyzes customer shopping behavior using transactional data to uncover actionable business insights. The analysis focuses on understanding revenue drivers, customer segments, discount effectiveness, product performance, and subscription impact to support data-driven decision-making.

The project is implemented using **Python (Jupyter Notebook)** for data analysis and visualization, and **PostgreSQL** for structured querying and advanced SQL-based insights.

---

## 🧾 Dataset Summary

* **Total Transactions:** 3,900 purchases
* **Features:** 18 data points per record
* **Product Types:** 25
* **Categories:** 4
* **Key Attributes:**

  * Customer demographics
  * Purchase amount and frequency
  * Discount usage
  * Subscription status
  * Product categories and ratings

---

## ⚙️ Tech Stack

* **Programming Language:** Python
* **Environment:** Jupyter Notebook
* **Database:** PostgreSQL
* **Libraries Used:**

  * pandas – data cleaning, transformation, and analysis using DataFrames
  * numpy – numerical operations
  * psycopg2 / sqlalchemy – PostgreSQL connectivity

---

## 🔄 Data Preparation & Processing

1. **Data Loading & Exploration**
   Imported raw data and reviewed structure, distributions, and summary statistics.

2. **Missing Value Handling**
   Imputed 37 missing review ratings using category-specific median values.

3. **Column Standardization**
   Renamed columns using `snake_case` for consistency and readability.

4. **Feature Engineering**

   * Created customer age groups
   * Derived purchase frequency metrics
   * Segmented customers based on buying behavior

5. **Database Integration**
   Loaded cleaned data into PostgreSQL for advanced SQL analysis and aggregation.

---

## 📊 Key Analysis & Insights

### 1️⃣ Revenue by Gender

* **Male Customers:** $157,890 (68%)
* **Female Customers:** $75,191 (32%)

➡ Male customers contribute more than double the revenue, indicating opportunities for gender-targeted campaigns.

---

### 2️⃣ Smart Discount Users

* **839 customers** used discounts but still spent **above average**
* Average purchase: **$60**
* Discount users spent between **$64–$97**
* Represent **21%** of total customers

➡ Discounts successfully attract high-value customers; optimization is needed to protect margins.

---

### 3️⃣ Top-Rated Products

| Rank | Product | Avg Rating |
| ---- | ------- | ---------- |
| 1    | Gloves  | 3.86       |
| 2    | Sandals | 3.84       |
| 3    | Boots   | 3.82       |
| 4    | Hat     | 3.80       |
| 5    | Skirt   | 3.78       |

➡ These products should be prioritized in promotions and recommendations.

---

### 4️⃣ Customer Segmentation

| Segment   | Definition     | Customers | Share |
| --------- | -------------- | --------- | ----- |
| New       | 1 purchase     | 83        | 2%    |
| Returning | 2–10 purchases | 701       | 18%   |
| Loyal     | 10+ purchases  | 3,116     | 80%   |

➡ A strong loyal customer base highlights effective retention but limits new customer inflow.

---

### 5️⃣ Subscription Analysis

* **Subscribers:** 1,053 (27%)
* **Non-Subscribers:** 2,847 (73%)
* Repeat buyers (5+ purchases):

  * Subscribers: 958
  * Non-subscribers: 2,518

➡ Significant potential exists to convert repeat non-subscribers into subscribers.

---

### 6️⃣ Revenue by Age Group

* Young adults contribute the highest revenue
* Middle-aged customers follow closely
* Revenue contribution is balanced across age segments

➡ Age-based personalization can further optimize marketing ROI.

---

## 💡 Strategic Recommendations

* **Boost Subscriptions**
  Introduce exclusive benefits to convert the 73% non-subscriber base.

* **Strengthen Loyalty Programs**
  Incentivize repeat purchases to sustain the loyal segment.

* **Optimize Discount Strategy**
  Focus discounts on high-value users while protecting profit margins.

* **Highlight Top Products**
  Promote top-rated items such as Gloves, Sandals, and Boots.

* **Targeted Marketing**
  Prioritize young adults and express shipping users for higher ROI.

---

## 📁 Project Structure (Suggested)

```
customer-shopping-analysis/
│
├── notebooks/
│   └── customer_analysis.ipynb
├── sql/
│   └── analysis_queries.sql
├── data/
│   └── cleaned_customer_data.csv
├── visuals/
│   └── charts_and_graphs/
├── README.md
```

---

## 🚀 How to Run the Project

1. Clone the repository
2. Install required Python libraries
3. Set up PostgreSQL and update connection credentials
4. Run the Jupyter notebook for analysis and visualization
5. Execute SQL scripts for database insights


## 📌 License

This project is for educational and portfolio purposes.

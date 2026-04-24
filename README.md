# 📊 Marketing Campaign Analysis (EDA Project)

## 📌 Objective
The goal of this project is to perform **Exploratory Data Analysis (EDA)** on a marketing dataset to understand customer behavior and identify **which marketing campaigns (channels) deliver the highest ROI**.

Instead of building a machine learning model, this project focuses on answering **"why customers respond"** and provides **data-driven recommendations** for budget allocation.

---

## 📂 Dataset
The dataset contains information about:
- Customer demographics (Age, Income, Education, Marital Status)
- Purchase behavior (Web, Store, Catalog)
- Product spending (Wine, Fruits, Meat, etc.)
- Campaign responses (AcceptedCmp1–5, Response)

---

## 🧹 Data Cleaning Steps
- Fixed delimiter issue (`;` separated values)
- Removed duplicate records
- Converted date column (`Dt_Customer`) to datetime format
- Handled missing values:
  - Filled missing `Income` with median
- Created new features:
  - **Age**
  - **Total Spend**
  - **Total Purchases**
  - **Customer Tenure**
  - **Total Children**

---

## 🔧 Feature Engineering
New features created to improve analysis:
- `Total_Spend` → Total amount spent by customer
- `Total_Purchases` → Total purchases across all channels
- `Customer_Tenure` → Days since customer joined
- `Total_Children` → Kids + Teens at home

---

## 📊 Exploratory Data Analysis

### 1. Customer Insights
- Average income: ~52K
- Customers show consistent spending behavior across categories
- Repeat purchases are high → indicates strong retention

---

### 2. Funnel Analysis
- Compared:
  - **Web Visits**
  - **Total Purchases**

📌 Insight:
- Customers purchase more than they visit monthly → strong engagement and loyalty

---

### 3. Campaign Performance (ROI Proxy)
Measured using campaign acceptance rate:

| Campaign        | Performance |
|----------------|------------|
| Latest Campaign (Response) | ⭐ Highest (~15%) |
| Campaign 3,4,5 | Moderate (~7%) |
| Campaign 1     | Low (~6%) |
| Campaign 2     | ❌ Very Low (~1%) |

---

### 4. Customer Segmentation
- Spending varies by:
  - Education
  - Marital status
- Helps identify high-value customer groups

---

## 📈 Key Insights
- Recent campaigns perform significantly better
- Some campaigns are underperforming and wasting budget
- Customers are already active → focus on personalization

---

## 💡 Recommendations

### ✅ Increase Budget
- Recent / high-performing campaigns (Response)
- Campaigns similar to 3, 4, 5

### ⚠️ Optimize
- Campaign 1 → improve targeting or messaging

### ❌ Reduce / Stop
- Campaign 2 → very low ROI

---

## 🚀 Conclusion
- Shift from equal budget allocation to **performance-based marketing**
- Focus on **high ROI campaigns and customer segments**
- Prioritize **engagement and personalization over mass targeting**

---

## 🛠️ Tools Used
- Python
- Pandas
- Matplotlib

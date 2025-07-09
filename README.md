# 📊 Marketing Campaign Effectiveness Analysis: Facebook vs. AdWords

---

## 📝 Project Description

This project analyzes **daily ad campaign data from Facebook and AdWords for 2019** to determine which platform yields better performance in **conversions, clicks, and cost-effectiveness.**

Using **hypothesis testing, regression, cointegration, and EDA**, this project aims to help marketing teams allocate budgets effectively and **maximize ROI**.

---

## 🎯 Objectives

✅ Identify which platform (Facebook or AdWords) yields higher conversions.  
✅ Analyze cost-effectiveness trends using **Cost Per Conversion (CPC)**.  
✅ Examine the relationship between clicks and conversions using **correlation and regression**.  
✅ Determine **long-term stability between ad cost and conversions using cointegration analysis**.

---

## 🗂️ Dataset Details

**File:** [marketing_campaign.csv](marketing_campaign.csv)
**Rows:** 365 (daily data for 2019)  
**Columns:**
- Date
- Facebook: Ad Views, Clicks, Conversions, Cost per Ad, CTR, Conversion Rate, CPC
- AdWords: Ad Views, Clicks, Conversions, Cost per Ad, CTR, Conversion Rate, CPC

This dataset allows comprehensive analysis of **ad performance metrics** across platforms.

---

## ⚙️ Tools and Libraries

- **Python 3**
- Pandas, NumPy
- Matplotlib, Seaborn
- SciPy, Statsmodels
- Scikit-learn

---

## 📈 Project Workflow

### 1️⃣ Business Question
> **Which ad platform (Facebook vs. AdWords) is more effective in terms of conversions and cost-efficiency?**

---

### 2️⃣ Data Cleaning & Preprocessing
- Converted date columns to `datetime` type.
- Removed `%` and `$` symbols from numeric columns.
- Ensured proper numerical type conversion for analysis.

---

### 3️⃣ Exploratory Data Analysis (EDA)

✅ **Distribution Analysis:** Visualized clicks and conversions using histograms.  
✅ **Conversion Categories:** Classified conversions into:
- `<6`
- `6-10`
- `10-15`
- `>15`

✅ **Insights:**
- Facebook had more frequent higher conversion days.
- AdWords had more days with lower conversion counts.

---

### 4️⃣ Correlation Analysis

- Facebook: **0.87** (strong positive correlation between clicks and conversions).
- AdWords: **0.45** (moderate positive correlation).

✅ Indicates **clicks strongly predict conversions for Facebook.**

---

### 5️⃣ Hypothesis Testing (A/B Testing)

#### Hypothesis:
**H₀:** Facebook conversions ≤ AdWords conversions  
**H₁:** Facebook conversions > AdWords conversions

**Results:**
- Facebook mean conversions: **11.74**
- AdWords mean conversions: **5.98**
- p-value: `9.35e-134` (very small)

✅ **Reject H₀** → Facebook significantly outperforms AdWords in conversions.

---

### 6️⃣ Regression Analysis

> **Predicting Facebook conversions based on Facebook ad clicks using Linear Regression.**

- **R² Score:** 76.35% (good predictive power)
- **Insights:**
  - For 50 clicks → expect ~9 conversions
  - For 80 clicks → expect ~13.7 conversions

✅ Enables practical planning for ad campaigns based on expected clicks.

---

### 7️⃣ Cost Per Conversion (CPC) Trend Analysis

- Tracked monthly CPC trends.
- Found **May and November as lowest CPC months**, making them ideal for higher ad investments.

---

### 8️⃣ Cointegration Analysis

Checked for **long-term equilibrium between ad cost and conversions**.

✅ p-value < 0.05 → **Confirms a stable relationship**, supporting strategic budget allocation aligned with expected conversions.

---

## 🚀 Key Results

✅ Facebook is **more effective** for conversions and ROI.  
✅ Strong positive correlation between Facebook clicks and conversions.  
✅ Mondays and Tuesdays have higher conversions.  
✅ May and November are cost-effective months for ad spend.  
✅ Regression model provides actionable conversion predictions.  
✅ Long-term cost-conversion stability confirmed for budget optimization.

---

## 🩶 Recommendations

✅ **Prioritize Facebook** for ad campaigns to maximize conversions.  
✅ Schedule ads on **Mondays and Tuesdays** for higher effectiveness.  
✅ Allocate higher budgets during **May and November** for cost-efficient campaigns.  
✅ Use regression insights to **plan click goals aligned with conversion targets.**  
✅ Monitor cost-conversion stability for long-term budgeting.

---

## 💡 Why This Project Matters

This project demonstrates:
✅ **Practical application of statistics in marketing analytics.**  
✅ **A/B Testing using hypothesis testing for business decisions.**  
✅ **Predictive modeling and time-based analysis for cost optimization.**

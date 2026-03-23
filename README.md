# 📊 Exploratory Data Analysis (EDA) – Complete Checklist

A detailed step-by-step checklist to perform thorough EDA on any dataset.

---

## 1. 🧠 Problem Understanding
- Clearly define the business problem.
- Understand what needs to be solved.
- Identify:
  - **Target variable** (dependent variable)
  - **Input variables** (features)
- Know expected output (prediction, insight, dashboard).

---

## 2. 📥 Import Data & Setup
- Load dataset (CSV, Excel, Database, API).
- Import libraries:
  - `pandas` → data handling
  - `numpy` → numerical operations
  - `matplotlib` / `seaborn` → visualization

---

## 3. 🔍 Initial Data Inspection
- Check dataset shape (rows, columns).
- Preview data:
  - `head()` → first rows
  - `tail()` → last rows
- Check column names.
- Check data types: `info()`.
- Summary statistics: `describe()`.
- Identify numerical vs categorical columns.

---

## 4. 🧹 Data Cleaning
### Missing Values
- Detect: `isnull().sum()`
- Handle by:
  - Dropping rows/columns
  - Filling with mean / median / mode
  - Forward/backward fill

### Duplicates
- Detect duplicates
- Remove using `drop_duplicates()`

### Data Type Fixing
- Convert:
  - `string → datetime`
  - `object → category`
  - `int ↔ float`

### Standardization
- Fix inconsistent values:
  - `"Male", "male", "M" → "Male"`
  - Remove extra spaces, symbols

---

## 5. 📈 Univariate Analysis (Single Variable)
### Numerical Features
- Mean, median, standard deviation
- Min, max, quartiles
- Distribution:
  - Histogram
  - Boxplot  
**Goal:** Understand spread, skewness, outliers

### Categorical Features
- Value counts
- Unique categories
- Visualization:
  - Bar chart  
**Goal:** Understand frequency & dominance

---

## 6. 🔗 Bivariate Analysis (Two Variables)
### Numerical vs Numerical
- Correlation (positive/negative)
- Scatter plot

### Categorical vs Numerical
- Groupby aggregation (mean, sum, count)
- Boxplot comparison

### Categorical vs Categorical
- Crosstab / frequency table
- Stacked bar chart  
**Goal:** Identify relationships & trends

---

## 7. 🔥 Multivariate Analysis (Multiple Variables)
- Correlation matrix
- Heatmap visualization
- Pairplot (all variable relationships)  
**Goal:** Detect complex interactions & patterns

---

## 8. ⚠️ Outlier Detection
- Methods:
  - Boxplot
  - IQR method
  - Z-score
- Decide:
  - Remove outliers
  - Cap (winsorization)
  - Keep (if valid data)

---

## 9. ⚙️ Feature Engineering
- Create new features:
  - Ratios (e.g., profit/revenue)
  - Aggregations (sum, avg)
  - Date features (year, month, day, weekday)
- Convert categorical variables:
  - Label encoding
  - One-hot encoding

---

## 10. 🔄 Feature Transformation
- Normalize (scale 0–1)
- Standardize (mean = 0, std = 1)
- Log transformation (for skewed data)  
**Goal:** Improve model performance & distribution

---

## 11. ⚖️ Check Data Imbalance (Classification)
- Analyze target variable distribution.
- If imbalanced:
  - Oversampling (SMOTE)
  - Undersampling

---

## 12. 📊 Visualization & Storytelling
- Use clear charts:
  - Bar charts
  - Line charts
  - Heatmaps
- Focus on:
  - Trends
  - Comparisons
  - Patterns  
**Tip:** Avoid clutter, keep it simple & meaningful

---

## 13. 🧾 Insights Summary
- Key findings from analysis
- Important patterns & relationships discovered
- Business insights:
  - What does it mean?
  - Why does it matter?

---

## 14. ✅ Final Dataset Preparation
- Clean, structured dataset ready for:
  - Machine learning models
  - Dashboards (Power BI, Tableau)
  - Reports

---

## ⚡ Reality Tip
EDA is **not linear** — you’ll repeat:
`Cleaning ↔ Analysis ↔ Visualization`  
It’s an iterative process.

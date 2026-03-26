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
<br>
  <hr>
  <hr>
<br>
## Univariate Analysis
Har single column ko deeply samajhna jahan hum distribution, missing values aur data behavior analyze kartay hain. Yeh Data Analyst ke liye foundation hai jo accurate analysis ki base banata hai.

## Bivariate Analysis
Do variables ke darmiyan relationship explore ki jati hai jahan trends aur dependencies identify hoti hain. Yeh step insights aur business understanding generate karne ke liye core hai.

## Visualization & Insights
Data ko charts aur visuals ke zariye represent kar ke clear insights nikaalay jatay hain. Yeh Data Analyst ki main value hoti hai jo raw data ko decision-making main convert karti hai.

## Outlier Detection
Extreme values ko identify kiya jata hai jo analysis ko distort kar sakte hain. Analyst level par inhein detect karna aur samajhna zaroori hota hai.

## Data Imbalance Check
Category distribution ko check kiya jata hai taake bias identify ho jo insights ko mislead kar sakta hai. Basic awareness Data Analyst ke liye kaafi hoti hai.

## Feature Transformation
Data ko simple form main convert kiya jata hai jaise encoding ya basic scaling taake analysis easy ho. Advanced transformation Data Scientist ka domain hota hai.

## Multivariate Analysis
Multiple variables ke combined effect ko samajhne ki basic understanding rakhi jati hai. Deep statistical modeling Data Analyst ke liye zaroori nahi hoti.
<br>
<hr>
<hr>
<br>
Mean (Average)
Data ke tamam values ka average jo overall central value batata hai aur general trend ko represent karta hai.

## Median
Sorted data ka beech wala point jo extreme values (outliers) ke effect se bach kar real center show karta hai.

## Mode
Wo value jo sab se zyada repeat hoti hai aur most frequent behavior ko represent karti hai.

## Count
Total number of observations jo dataset ke size aur data availability ko show karta hai.

## Sum
Tamam values ka total jo overall magnitude aur volume ko represent karta hai.

## Min
Sab se chhoti value jo data ke lower boundary aur extreme low ko define karti hai.

## Max
Sab se bari value jo data ke upper boundary aur extreme high ko define karti hai.

## Range
Max aur Min ka difference jo data ke spread aur variability ka basic idea deta hai.

## Variance (Var)
Data ke spread ka measure jo batata hai ke values mean se kitni door phel rahi hain.

## Standard Deviation (Std)
Variance ka square root jo real units main data ke deviation ko easy tarike se samjhata hai.

## Quantile
Data ko equal parts main divide karta hai jahan har portion distribution ka specific segment represent karta hai.

## Quartiles (Q1, Q2, Q3)
Data ko 4 parts main divide karta hai jahan Q2 median hota hai aur Q1/Q3 spread ko detail main show kartay hain.

## IQR (Interquartile Range)
Q3 - Q1 jo middle 50% data ka spread batata hai aur outlier detection main use hota hai.

## Skewness
Distribution ka jhukao batata hai ke data left ya right side par zyada tilted hai.

## Kurtosis
Distribution ki peak aur tails ka shape batata hai ke data normal hai ya heavy/light tails rakhta hai.

## Correlation
Do variables ke darmiyan relationship ki strength aur direction ko measure karta hai.

## Covariance
Do variables ke sath move karne ka trend batata hai lekin scale dependent hota hai.

## Unique
Unique values ki ginti jo data ke diversity aur categorical spread ko show karti hai.

## Value Counts
Har category ki frequency batata hai jo categorical analysis ke liye useful hota hai.

## Percentile
Specific percentage position batata hai jahan koi value dataset main stand karti hai.

## Z-Score
Har value ka standardized distance mean se batata hai jo outlier detection aur normalization main use hota hai.

## Distribution
Data ka overall shape (normal, skewed, uniform) jo behavior aur patterns ko samajhne main help karta hai.

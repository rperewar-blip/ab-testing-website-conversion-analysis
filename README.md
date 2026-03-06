# A/B Testing Analysis for Website Conversion

## Project Overview

This project analyzes an A/B test experiment comparing the performance of an **old landing page** and a **new landing page**. The objective is to determine whether the new page improves user conversion rates.

The analysis follows a complete experimentation workflow including data cleaning, exploratory analysis, statistical hypothesis testing, and business recommendations.

---

## Business Question

Should the company replace the existing landing page with the new version based on conversion performance?

---

## Dataset Description

The dataset contains user-level observations from an A/B testing experiment.

Columns include:

| Column | Description |
|------|-------------|
| user_id | Unique user identifier |
| timestamp | Time of experiment interaction |
| group | Experiment group (control or treatment) |
| landing_page | Page shown to the user |
| converted | Whether the user converted (1) or not (0) |

---

## Tools Used

- Python
- Pandas
- Matplotlib
- SciPy
- Jupyter Notebook

---

## Data Cleaning

Before analysis, the dataset was cleaned by:

- Removing mismatched experiment assignments  
- Ensuring control group saw only the old page  
- Ensuring treatment group saw only the new page  
- Removing duplicate users  

This ensures a valid A/B testing comparison.

---

## Conversion Rate Results

| Group | Users | Conversions | Conversion Rate |
|------|------|-------------|----------------|
| Control | 145,274 | 17,489 | 12.04% |
| Treatment | 145,310 | 17,264 | 11.88% |

The control group achieved a slightly higher conversion rate.

---

## Statistical Testing

Two statistical methods were used to validate the result.

### Two-Proportion Z-Test

- Z-score: -1.3109  
- p-value: **0.1899**

### Chi-Square Test

- Chi-square statistic: **1.703566**
- p-value: **0.191822**

---

## Interpretation

Since both p-values are greater than **0.05**, we fail to reject the null hypothesis.

This means there is **no statistically significant difference** between the old page and the new page.

---

## Final Business Recommendation

Based on the experiment results, the company should **not replace the existing landing page** with the new version at this time.

The observed difference in conversion rates is not statistically significant and may be due to random variation.

---


---

## Key Skills Demonstrated

- A/B testing analysis
- Data cleaning and validation
- Conversion rate analysis
- Statistical hypothesis testing
- Business decision making from experimental data

---

## Author

**Rishabh Perewar**

Data Analytics / Business Analytics Portfolio

# Customer Satisfaction Analysis

## About -
This project analyzes customer support data to understand customer satisfaction.

[Dataset Used](https://github.com/bhartijonwal/Python-analysis-for-customer-Satisfaction/blob/main/Customer_support_data.csv) — Dataset used in this project.

[Python Analysis (Code)](https://github.com/bhartijonwal/Python-analysis-for-customer-Satisfaction/blob/main/Customer%20Project.ipynb) — Data analysis, Exploratory Data Analysis and Visualization

## Tools
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

# Problem Statement
In e-commerce, customer support feedback is generated at high volume and is hard to evaluate manually. This project converts raw feedback into structured insights that help monitor service quality and improve customer experience.

# Dataset Snapshot
- **Shape:** 85,907 rows × 20 columns
- **Example columns:** `Customer Remarks`, `Category`, `Sub-category`, `Item_price`, `Agent_name`, `CSAT Score`
- **Missing data highlights:**
  - `connected_handling_time`: ~99% missing
  - `order_date_time`, `Customer_City`, `Product_category`: ~70–80% missing
    
# What Was Done
## 1) Data Cleaning & Preprocessing
- Treated missing and inconsistent values
- Converted date fields to datetime type
- Dropped non-useful columns (for example, `Unique_id`)

## 2) Exploratory Data Analysis (EDA)
- Used bar charts, heatmaps, and count plots
- Studied trends, distributions, and basic relationships
- Detected outliers in `Item_price` with IQR and applied clipping

## 3) Feature Engineering & Preparation
- Addressed class imbalance with `RandomOverSampler`
- Used one-hot encoding for low-cardinality features
- Used binary encoding for high-cardinality features (such as `Agent_name`, `Manager`)
- Standardized numeric features using `StandardScaler`

## Key Insights
- Agent shift, tenure, and product category show meaningful association with CSAT.
- Class imbalance handling improved data readiness for downstream modeling.
- Visual analysis made customer sentiment patterns easier to interpret.

## Quick Q&A
- Main challenge?
   High missing-value ratios and class imbalance in satisfaction scores.
- **Why binary encoding?** It handles high-cardinality features efficiently without large dimensional expansion.
- **Why IQR for outliers?** It is robust for skewed data and less sensitive to extreme values than Z-score in this context.

## Conclusion
The project demonstrates a practical analytics pipeline for extracting actionable CSAT insights from support data. The workflow can be extended into prediction systems and business dashboards.

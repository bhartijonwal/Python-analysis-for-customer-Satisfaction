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
    
  <img width="559" height="244" alt="image" src="https://github.com/user-attachments/assets/48fc7781-dbb2-46b5-beab-e42bf27d245c" />

    
# What Was Done
## 1) Data Cleaning & Preprocessing
- Treated missing and inconsistent values
- Converted date fields to datetime type
- Dropped non-useful columns (for example, `Unique_id`)

## 2) Exploratory Data Analysis (EDA)
- Used bar charts, heatmaps, and count plots
- Studied trends, distributions, and basic relationships
- Detected outliers in `Item_price` with IQR and applied clipping



## Key Insights
- Agent shift, tenure, and product category show meaningful association with CSAT.
  <img width="570" height="310" alt="image" src="https://github.com/user-attachments/assets/1a091fea-4ff5-41eb-9917-0c8d89fa95e6" />

- Class imbalance handling improved data readiness for downstream modeling.
  <img width="548" height="245" alt="image" src="https://github.com/user-attachments/assets/80aa254e-a49e-42a2-9b1f-045db2442ab5" />

- Visual analysis made customer sentiment patterns easier to interpret.
<img width="548" height="290" alt="image" src="https://github.com/user-attachments/assets/aa759092-9059-46c7-b518-ca7e698aea8f" />

<img width="541" height="385" alt="image" src="https://github.com/user-attachments/assets/a147e30e-d890-4e8f-bdde-24fe9d7dafa2" />


## Quick Q&A
- **Main challenge?**
   High missing-value ratios and class imbalance in satisfaction scores.
- **Why binary encoding?**
  It handles high-cardinality features efficiently without large dimensional expansion.
- **Why IQR for outliers?**
  It is robust for skewed data and less sensitive to extreme values than Z-score in this context.

  <img width="451" height="377" alt="image" src="https://github.com/user-attachments/assets/043024f0-d685-404c-8a5a-ec5ea00cfc01" />


## Conclusion
The project demonstrates a practical analytics pipeline for extracting actionable CSAT insights from support data. The workflow can be extended into prediction systems and business dashboards.

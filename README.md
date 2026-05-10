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

Project Summary
This project focuses on exploring and analyzing customer support feedback data from Flipkart to uncover patterns and insights related to customer satisfaction (CSAT). The objective was to perform end-to-end data processing and visual analytics to help understand key drivers behind customer sentiment and satisfaction.

🔍 Problem Statement
In a competitive e-commerce landscape, understanding customer satisfaction is crucial. Flipkart receives a large volume of support feedback that is difficult to analyze manually. This project transforms that raw feedback into structured insights to help monitor, evaluate, and improve customer experience.

📂 Dataset Overview
Size: 85,907 rows × 20 columns
Key Features:
Customer Remarks, Category, Sub-category, Item_price, Agent_name, CSAT Score, etc.
Missing Data:
connected_handling_time: ~99% missing
order_date_time, Customer_City, Product_category: 70–80% missing
🛠️ Key Steps & Techniques
🔧 Data Cleaning & Preprocessing
Handled missing values and inconsistent entries.
Converted object types to datetime for date fields.
Dropped irrelevant columns (Unique_id).
📊 Exploratory Data Analysis (EDA)
Uncovered trends, correlations, and distributions using:
Bar Charts
Heatmaps
Count Plots
Identified outliers in Item_price using IQR Method, then applied clipping to manage them.
🧪 Statistical Testing
Applied IQR-based outlier detection.
Considered correlation analysis to validate data relationships.
⚖️ Handling Class Imbalance
Used RandomOverSampler to balance CSAT score distribution.
🔐 Encoding Techniques
One-Hot Encoding: For low-cardinality categorical features.
Binary Encoding: For high-cardinality columns (e.g., Agent_name, Manager).
📈 Scaling
Applied StandardScaler to normalize numerical features (mean = 0, std = 1).
✨ Key Insights
Agent shift, tenure, and product category showed significant correlation with CSAT.
Imbalanced class distribution was handled effectively for reliable modeling.
Visualizations provided strong clarity on customer sentiment patterns.
❓ Q&A
Q: What was the main challenge?
A: High missing value ratios and imbalanced satisfaction scores.

Q: Why binary encoding for some features?
A: To handle high-cardinality columns efficiently without expanding feature space.

Q: Why IQR over Z-score?
A: IQR is less sensitive to extreme values and more robust for skewed data.

✅ Conclusion
This project demonstrates how data analytics can unlock key insights from customer support feedback using structured cleaning, visualization, and analysis. The pipeline is scalable for further ML-based satisfaction prediction or dashboard integration.

🚀 Future Work
Integrate real-time dashboard with Streamlit or Power BI.
Deep dive into sentiment analysis using NLP.
Deploy automated alert system for low CSAT detection.

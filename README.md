# Walmart Sales Data Analysis & Dashboard

## 📌 Project Overview
This project focuses on analyzing historical sales data from 45 Walmart stores located in various regions. The dataset contains weekly sales data, promotional markdowns, and macroeconomic indicators. 

The primary goal of this project is to perform end-to-end data processing starting from data cleaning in **Python**, moving towards building a Star Schema data model, and an interactive Business Intelligence dashboard using **Power BI**. This allows stakeholders to explore sales trends, evaluate promotional campaigns, and understand the impact of external factors on revenue.

## 🛠️ Tech Stack & Methodologies
* **Data Processing & Statistics:** Python (Pandas, NumPy, SciPy for A/B Testing).
* **Business Intelligence:** Power BI (DAX, Star Schema Data Modeling, Dynamic Formatting).
* **Methodologies:** Exploratory Data Analysis (EDA), A/B Testing (T-Test), UI/UX Dashboard Design.
## 🛠️ Problem Statement & Analysis Type
Retail datasets often suffer from missing values, hidden returns (negative sales), and complex promotional cycles. This project applies the following analytical approaches:
* **Descriptive Analytics:** What were our historical sales? Identifying top-performing stores and departments.
* **Diagnostic Analytics:** Why did sales spike or drop? Isolating the impact of holiday weeks and tracking the volume of product returns.
* **Correlation Analysis (Macroeconomics):** How sensitive is our retail performance to external economic factors like fuel prices, unemployment, and inflation (CPI)?
## **💡 Key Insights:**
* **The "Size vs. Efficiency" Paradox:** While Type A (mega-stores) naturally dominate the overall revenue share, the scatter plot reveals that physical size does not strictly dictate efficiency. 
* **The "Store 10" Phenomenon (Type B Outlier):** The scatter plot clearly isolates Store 10 (a Type B format) positioned significantly above the trendline. Despite having a smaller physical footprint than Type A mega-stores, it generates exceptional sales volume, proving to be a highly efficient positive outlier.
* **Return Rate Stability:** The overall return rate is remarkably low (0.3%), indicating strong product satisfaction and minimal revenue leakage.
* **Revenue Concentration:** A specific cluster of top-tier branches (e.g., Stores 20, 4, 14) disproportionately drives the total $6.74bn revenue.

**🚀 Actionable Recommendations:**
* **Investigate Store 10's Blueprint (Center of Excellence):** Store 10 should be treated as a case study. Management must investigate its operational blueprint—whether it's driven by local demographics, high inventory turnover, or exceptional store management—and replicate this winning model across other Type B and underperforming Type A stores.
* **Optimize Floor Space Over Expansion:** Before investing capital into expanding the physical footprint of smaller stores, maximize the Revenue per Sq Ft metric by adopting the layout and product mix strategies of highly efficient branches.

## 🎯 Questions to be Answered (Business Objectives)
This project is designed to answer the following strategic business questions:

1. **Performance & Space Efficiency:** Which stores and departments generate the highest revenue, and do larger stores (Type A) utilize their square footage more efficiently than smaller ones?
2. **Seasonality & Holiday Impact:** What is the exact volume of incremental sales (Uplift) generated during major holiday weeks (Super Bowl, Labor Day, Thanksgiving, Christmas) compared to baseline weeks?
3. **MarkDown ROI:** Do the promotional campaigns (MarkDowns 1-5) implemented after November 2011 significantly drive sales, and which specific markdown is most effective before the holidays?
4. **Macroeconomic Sensitivity:** How do external factors such as the Consumer Price Index (CPI), Unemployment Rate, and Fuel Prices correlate with weekly store performance?
5. **Returns Analysis (Hidden Losses):** Which departments suffer from the highest volume of negative sales (returns), and how does this impact the net revenue of the respective stores?

---
*Note: Data cleaning and preparation were performed using Python (Pandas), and the cleaned master datasets have been exported for Data Modeling in Power BI.*

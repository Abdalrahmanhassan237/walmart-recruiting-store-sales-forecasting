# Walmart Sales Data Analysis & Dashboard

**[🔗 Click Here to View the Interactive Power BI Dashboard][(https://app.powerbi.com/view?r=eyJrIjoiYmNmMDJkMDYtZGY5MS00MWZjLTg4Y2MtNWVlMDY1ZWU1NWViIiwidCI6IjJiYjZlNWJjLWMxMDktNDdmYi05NDMzLWMxYzZmNGZhMzNmZiIsImMiOjl9)]**

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

## 🎯 Questions to be Answered (Business Objectives)
This project is designed to answer the following strategic business questions:
1. **Performance & Space Efficiency:** Which stores and departments generate the highest revenue, and do larger stores (Type A) utilize their square footage more efficiently than smaller ones?
2. **Seasonality & Holiday Impact:** What is the exact volume of incremental sales (Uplift) generated during major holiday weeks compared to baseline weeks?
3. **MarkDown ROI:** Do the promotional campaigns implemented significantly drive sales, and are they statistically significant?
4. **Macroeconomic Sensitivity:** How do external factors such as Unemployment Rate and Temperature correlate with weekly store performance?
5. **Returns Analysis (Hidden Losses):** Which departments suffer from negative sales (returns), and how does this impact net revenue?

---

## 📊 Dashboard Pages & Insights

### 1️⃣ Page 1: Executive Overview & Store Efficiency
**❓ Strategic Question Answered:** Which stores make the most money, and does a bigger store size mean better sales?

**🛠️ Key Visuals:**
* **KPI Cards:** Quick look at Total Sales ($6.74bn), Sales per Sq Ft ($1,149), and the Return Rate (0.3%).
* **Scatter Plot:** Shows the relationship between Store Size and Total Sales to spot top performers.
* **Bar Chart:** Highlights the Top 15 stores by revenue.
* **Donut Chart:** Shows sales share by store type (A, B, C) using custom tooltips for cleaner design.

**💡 Key Insights:**
* **Size Isn't Everything:** While the biggest stores (Type A) bring in the most total revenue, the scatter plot shows that smaller stores can be highly efficient too.
* **The "Store 10" Outlier:** Store 10 (a Type B store) is a massive success. Despite being smaller, it sits way above the trendline, making much more money than expected for its size.
* **Healthy Return Rate:** The overall return rate is very low (0.3%), meaning lost revenue from returns is well under control.
* **Top Earners:** A small group of branches (like Stores 20, 4, and 14) drives a huge portion of the $6.74bn total sales.

**🚀 Actionable Recommendations:**
* **Learn from Store 10:** Management should study exactly why Store 10 is so successful (e.g., better layout, product mix, or management) and apply its strategy to other branches.
* **Focus on Efficiency:** Instead of just building bigger stores, the company should focus on increasing the "Sales per Sq Ft" in current stores to match the top performers.
### 2️⃣ Page 2: Seasonality & External Impacts
**❓ Strategic Question Answered:** How much do holidays boost our revenue, and do external economic factors (like unemployment) affect our sales?

**🛠️ Key Visuals:**
* **KPI Cards:** Compares Average Holiday Sales ($17,036) vs. Non-Holiday Sales ($15,901), showing a 7.13% Holiday Uplift, alongside the Average Unemployment Rate.
* **Monthly Sales Heatmap:** A color-coded matrix replacing a standard table, making it instantly clear which months generate the most revenue across different years.
* **Butterfly Chart:** Compares the impact of holidays vs. regular days across the three store types (A, B, and C).
* **Revenue vs. Unemployment Trend (Line & Column Chart):** Tracks total sales over time against the shifting unemployment rate to see if a tough economy hurts Walmart's sales.

**💡 Key Insights:**
* **The Holiday Boost:** Major holidays reliably increase average weekly sales by about 7.13%. 
* **December is King:** The Heatmap clearly highlights December as the most profitable month every single year, proving a massive end-of-year seasonal spike.
* **Type A Dominates Holidays:** Larger stores (Type A) capture the vast majority of the extra holiday spending compared to Types B and C.
* **Economic Resilience:** The Unemployment vs. Revenue chart shows how sales respond to economic changes. Interestingly, as a discount retailer, Walmart maintains strong sales even when unemployment fluctuates, proving its business model is highly resilient.

**🚀 Actionable Recommendations:**
* **Smart Staffing & Inventory:** Since December and holiday weeks show a massive spike, management must aggressively scale up warehouse inventory and temporary staffing right before these periods to avoid out-of-stock issues.
* **Targeted Holiday Promotions:** Since Type A stores see the biggest holiday jumps, the marketing budget for holiday campaigns should be heavily focused on these specific mega-stores to maximize ROI.
### 3️⃣ Page 3: Department & Markdown Analysis (A/B Testing)
**❓ Strategic Question Answered:** Which specific departments are making or losing money, and do our promotional discounts (Markdowns) actually work?

**🛠️ Key Visuals:**
* **Dynamic KPI Cards:** Instantly highlights the Top Performing Department (e.g., Dept 92) and the Bottom Performing Department (e.g., Dept 47) with built-in trend lines.
* **A/B Test Result Card:** A custom metric showing the actual sales lift (e.g., +2.70%) driven by a specific promotion (Markdown 1), confirming if it's "Statistically Significant".
* **Decomposition Tree:** An interactive AI visual that breaks down Total Sales step-by-step (by Store Type ➔ Department ➔ Store) to find exactly where money is coming from.
* **Top 10 Departments Bar Chart:** A clean view of the highest-earning departments across the company.

**💡 Key Insights:**
* **Promotions Actually Work:** The A/B Test proves that "MarkDown 1" was highly successful for Type A stores, generating a real +2.70% lift in sales rather than just a random spike.
* **The "Heavy Lifters":** A few specific departments (like Dept 92 and 95) consistently bring in the most cash across almost all store locations.
* **Catching the "Money Leaks":** The Bottom KPI card dynamically catches departments with negative sales (like Dept 47). Negative sales mean high product return rates or operational losses that are silently eating away at profits.

**🚀 Actionable Recommendations:**
* **Scale Winning Promotions:** Since Markdown 1 is statistically proven to boost sales in Type A stores, the marketing team should confidently increase the budget for this specific promotion and test it in Type B stores.
* **Audit Losing Departments:** Management must immediately investigate bottom-performing departments (like Dept 47). High return rates mean they need to improve product quality, change suppliers, or completely drop those product lines to stop the bleeding.
### 4️⃣ Page 4: Macroeconomic & Feature Sensitivity (Key Influencers)
**❓ Strategic Question Answered:** Which hidden external factors (like weather or economy) are most likely to drive our sales down?

**🛠️ Key Visuals:**
* **Key Influencers (AI Visual):** An advanced Machine Learning visual built into Power BI that analyzes all dataset features simultaneously to rank what factors are mathematically most likely to cause a decrease in Total Sales.

**💡 Key Insights:**
* **The Unemployment "Danger Zone":** Sales don't just drop linearly with unemployment. The AI identified a specific danger zone: when unemployment hits between 9.0% and 10.6%, average store sales drop significantly (by over $400K).
* **Weather Sensitivity:** Colder weather has a direct negative impact. When the temperature drops to 19.83 or lower, average sales decrease by roughly $368K, likely due to reduced foot traffic.
* **The "Discount Haven" Effect:** Interestingly, in areas where unemployment is extremely high (over 10.6%), sales actually spike upward. This suggests that in severe economic conditions, Walmart becomes the ultimate go-to destination for price-sensitive shoppers.

**🚀 Actionable Recommendations:**
* **Targeted Marketing by Region:** The marketing team should launch aggressive promotional campaigns specifically in regions where unemployment is approaching that 9.0% - 10.6% "danger zone" to prevent the expected $400K drop in revenue.
* **Weather-Responsive Supply Chain:** Anticipate lower overall sales during colder months (under 19.8 degrees) and adjust inventory ordering algorithms accordingly to prevent overstocking and reduce warehousing costs.
---
*Note: Data cleaning and preparation were performed using Python (Pandas), and the cleaned master datasets have been exported for Data Modeling in Power BI.*

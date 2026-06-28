# DecodeLab-project2
Eploratort data analysis
# 📈 Project 2: Exploratory Data Analysis (EDA)
 **Analyst:** Aleke James

##  Objective
Analyzed the cleaned e-commerce dataset to uncover patterns, trends, and operational risks. Focused on translating raw statistics into actionable business intelligence regarding revenue drivers, coupon effectiveness, and order failure root causes.

## 📊 Key Statistical Findings

### 1. Revenue & Seasonality
-   **Peak Revenue Month:** June ($154,239), driven by end-of-fiscal-year spending.
-   **Lowest Revenue Month:** September ($66,054), indicating a need for targeted Q3 campaigns.
-   **Top Product:** Tablets lead in unit volume across 4 months; Laptops dominate Q4.

### 2. Coupon Effectiveness
-   **FREESHIP is King:** Generated highest total revenue ($318k) despite similar order counts to "No Coupon." Suggests free shipping drives higher basket sizes than percentage discounts.
  
### 3. Critical Risk: Order Failures
-    Combined Cancelled (242) + Returned (243) orders represent a massive revenue leak.
-   **Product Quality Issue:** Chairs have the highest cancellation (~24.1%) AND return rates (~24.1%), suggesting manufacturing or description issues.
-   **The "Full-Price" Paradox:** "No Coupon" orders had the highest absolute volume of returns (75), implying full-price buyers have stricter satisfaction thresholds.

## 🔍 Methodology
-   **Descriptive Statistics:** Mean, median, count profiling for all numerical columns.
-   **Outlier Analysis:** Boxplots for visual inspection 
-   **Root Cause Analysis:** Cross-tabulation of `OrderStatus` against `Product`, `CouponCode`, and `UnitPrice`.
-   **Time-Series Analysis:** Monthly revenue and sales trend visualization by product category.

## 🖼️ Visualizations Generated
-    Outlier detection across numeric columns
-    Revenue seasonality and product performance over time

## 💡 Strategic Recommendations
1.  **Quality Audit:** Immediate review of Chair inventory/descriptions to reduce 24% failure rate.
2.  **Checkout Optimization:** Implement installment payments for high-ticket items to reduce price-driven cancellations.
3.  **Promotion Shift:** Reallocate budget from `SAVE10` to `FREESHIP` .
4.  **Seasonal Planning:** Launch "Back-to-School" or "Autumn Refresh" campaigns in August/September to mitigate revenue dip.

##  Tools & Technologies
-   **Python:** Pandas, Matplotlib, Seaborn
-   **Analysis Type:** Descriptive Statistics, Root Cause Analysis, Time-Series

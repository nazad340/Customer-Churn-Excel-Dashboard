# Customer Churn Dashboard (Excel)

## Project Overview
This project is a professional-grade interactive dashboard built in Excel to analyze and visualize customer churn data. The goal was to transform raw customer data into actionable insights for a telecommunications company to help identify why customers are leaving.

## 📊 Key Features
* **KPI Scorecard:** Real-time tracking of Total Customers, Churn Rate, Revenue, and Average Monthly Charges.
* **Contract Analysis:** A combo chart (Clustered Column + Line) showing churn rates by contract duration.
* **Service Deep-Dive:** Analysis of churn trends based on Internet Service types (Fiber Optic vs. DSL).
* **Revenue Trending:** A smoothed line chart visualizing the monthly revenue growth over a 12-month period.
* **Payment Behavior:** A donut chart breakdown of customer payment methods.

## 🛠️ Technical Details
* **Dynamic Linking:** Utilized a "Calculation Sheet" architecture to keep the UI clean. KPI cards are dynamically linked to calculation cells using the Formula Bar.
* **Calculations:** * **Churn Rate:** Computed using `=COUNTIF(tbl_churn[Churn], "Yes") / COUNTA(tbl_churn[Churn])`.
    * **Revenue:** Calculated via structured table references: `=SUM(tbl_churn[Revenue])`.
* **Formatting:** Used custom currency and percentage formatting to ensure a professional UI/UX.
* **Interactivity:** Integrated Slicers (not shown in all previews) to allow for data filtering by category.
## 🚀 How to Use
1. Download the `Customer_Churn_Dashboard.xlsx` file.
2. Open in Microsoft Excel (Desktop version recommended).
3. If prompted, "Enable Content" to allow the Pivot Table and Slicer connections to function.

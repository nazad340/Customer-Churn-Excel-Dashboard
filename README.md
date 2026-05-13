Telco Customer Churn Analysis
==============================

I built this project to practice turning messy, real-world data into
something a business can actually use. The dataset comes from IBM and
contains information on 7,043 telecom customers — things like their
contract type, monthly charges, internet service, and whether they
eventually left the company.

The goal was simple: figure out who is churning, why, and how much it
is costing the business.


What I Built
------------
A multi-sheet Excel workbook that walks through the analysis like a
story — starting from a high-level executive summary and drilling down
into the details. Here is what each sheet covers:

Cover               The business problem, key numbers at a glance, and
                    a guide to the rest of the workbook.

Executive Dashboard The main view. KPI cards, churn breakdowns by
                    contract type, internet service, and customer tenure,
                    plus a callout panel with the five most important
                    findings.

Churn Deep Dive     A closer look at payment methods, service features,
                    senior citizen behavior, and billing type — with a
                    business interpretation for each finding.

Customer Segments   I built a simple risk scoring model that groups all
                    7,043 customers into four tiers (Critical, High,
                    Medium, Low) based on factors like contract type,
                    tenure, and payment method. Each tier has a
                    recommended action.

Revenue Impact      The business case section. Shows how much revenue
                    is leaking each month and models out what happens
                    if you reduce churn by 5%, 10%, 20%, or 35% —
                    including estimated ROI.

Raw Data            The full cleaned dataset with alternating row colors,
                    auto-filters on every column, and the Churn column
                    highlighted in red or green for quick scanning.


What I Found
------------
A few things really stood out in the data:

- Month-to-month customers churn at 42.7%. Customers on two-year
  contracts churn at just 2.8%. That gap alone explains most of the
  revenue loss.

- Fiber optic customers pay the highest monthly charges ($91.50 avg)
  but also churn the most (41.9%). High price and high churn together
  is a serious problem worth investigating.

- More than half of all churned customers left within their first six
  months. Onboarding is clearly broken.

- Customers paying by electronic check churn at 45.3%, nearly three
  times the rate of credit card users. Nudging them toward auto-pay
  could make a real difference.

- The company is losing around $139,000 in monthly recurring revenue
  to churn. Annualized, that is $1.67M walking out the door.


Tools and Techniques
--------------------
- Microsoft Excel (formatting, conditional coloring, structured layout)
- Cohort analysis across tenure buckets
- Churn rate segmentation across 10+ variables
- Custom risk scoring model (10 factors, 4 tiers)
- Customer LTV estimation by contract type
- Scenario modeling for retention investment ROI


How to Open It
--------------
1. Download Telco_Churn_Portfolio_Project.xlsx
2. Open in Microsoft Excel 2016 or later
3. Start on the Cover sheet and work through in order
4. Use the filters on the Raw Data sheet to explore on your own


Dataset
-------
IBM Watson Telco Customer Churn — publicly available dataset.
7,043 customers, 21 variables, no missing values after cleaning.

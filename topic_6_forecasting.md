---
marp: true
author: Marcelo Ortiz 
title: "Forecasting Analysis"
paginate: true
_paginate: false
header: 2023 | M. Ortiz  | Forecasting Analysis
_header: ""
date: 2023-07-11
math: mathjax
theme: custom-default
---
![bg left:60%](Slides/../topic_2_img/bg_1.png)
# Forecasting Analysis

Marcelo Ortiz

(UPF, BSE, BSM)

---
#  How to forecast financial statements:question:

1. Why do we need to forecast financial statements?
2. Step 1: Projected Income Statement
3. Step 2: Projected Balance Sheet
4. Sensitivity Analysis
---
# 1. Why do we need to forecast financial statements?
---
# 1. Why do we need to forecast financial statements?
Propective analysis is the process of forecasting the future performance of a company.

Managers use prospective analysis to:
- Evaluate the impact of different strategies, financing, and investment decisions on the company's future performance
- By doing so, they can foresee how investors and creditors will react to these decisions
---
Investors and creditors forecast financial statements because it allows them to:
- Estimate the future cash flows of the company
- Estimate the future value of the company

The forecast starts when the historical financial statements have been properly adjusted:
- eliminating transitory items in the income statement
- capitalizing (expensing) items that have been expensed (capitalized) by management
- capitalizing operating leases
- other forms of off-balance sheet financing
- and so on...

---
# 2. Step 1: Projected Income Statement
---
# 2. Step 1: Projected Income Statement
The projected income statement is the starting point of the prospective analysis
Step 1.1, we need an estimation of the company's expected sales growth rate:
- Easy approach: use the historical trend in sales growth rate
- More sophisticated approaches:
  - expected level of macroeconomic activity: using econometrics to link sales growth to GDP growth. If the economy is in a cyclical upturn, sales growth is expected to be higher than the historical average
  - product market competition: if the company is in a highly competitive industry, the company has no price-setting power and sales growth can easily decline
---
Step 1.2, we need to estimate the company's expected gross profit margin:
- Easy and most common approach: use the historical trend in gross profit margin
- As a subproduct, we can calculate the company's expected _cost of goods sold_ (COGS) as a _sales_ - _gross profit_ (step 1.3)

Let's jump to the example in MS Excel.

--- 
Step 1.4, we need to estimate the company's expected _selling, general, and administrative expenses_ (SG&A):
- it is reasonable to argue that a relevant portion of SG&A is varies with the company's sales
  - advertising and marketing expenses
  - sales commissions
  - salaries of salespeople
- it is also reasonable to argue that a relevant portion of SG&A is fixed
  - salaries of top management
  - depreciation and insurance of the company's headquarters
  - rent and insurance
  - and so on...

--- 
Problem: how to estimate the variable and fixed portions of SG&A?
- managers: easy, cost accounting and budgetting (later on this course)
- investors and creditors: kind of impossible
  - therefore, they use historical trend in SG&A as a percentage of sales (so, consider that all SG&A is variable)

 Let's jump to the example in MS Excel.

 --- 
 Step 1.5, we need to estimate the company's expected _depreciation and amortization_ (D&A):
 - we know that this fixed cost is a function of the company's gross PP&E at the beginning of the period
   - so, it is reasonable to predict future D&A is a fraction of gross PP&E
 - the underlying assumption is that the company will not significantly change its PP&E structure
   - for now, let's keep this assumption to understand the mechanics of forecasting

 Let's jump to the example in MS Excel.

 ---   
Step 1.6, we need to estimate the company's expected _interest expenses_:
- This is also a fixed cost, so the preduction is relatively easy if we assume no changes in debt structure
- we know that this fixed cost is a function of the company's debt at the beginning of the period


Step 1.7 we can calculate the company's expected _Income before tax_ as a _sales_ - _COGS_ - _SG&A_ - _D&A_ - _interest expenses_

---
Step 1.8, we need to estimate the company's expected _tax_expenses_:
- we know that this cost is a function of the company's income before tax
- if we know well the tax system of the country, we can estimate the company's expected TDA and TDL, and then calculate the company's expected tax expenses
- however, in practice, most of the analyst just use the effective tax rate (ETR) as a percentage of income before tax
  $$ \text{effective tax rate ETR} =\frac{\text{tax expenses}} {\text{income before tax}} $$

---
Step 1.9, we focus on extraordinary items and discontinued operations:
- by their very nature, these items are not expected to occur in the future
- so, it is not sensitive to use past values as forecasted values
- therefore, we just assume that these items will be zero in the future
  - there are, of course, exceptions to this rule, but we will not discuss them here
---
Step 1.10, we can calculate the company's expected _net income_ as a _income before tax_ - _tax expenses_ - _extraordinary items_ - _discontinued operations_

---
# 3. Step 2: Projected Balance Sheet
---
# 3. Step 2: Projected Balance Sheet
Step 2.1, estimate the company's expected _accounts receivable_:

$$\text{Accounts receivable turnover rate}=\frac{\text{Sales}}{\text{Accounts receivable balance}} $$

The forecast:
$$\text{Forcasted accounts receivable} =\frac{\text{Forecasted Sales}}{\text{Accounts receivable turnover rate}} $$
---
Step 2.2, estimate the company's expected _inventories_:
$$\text{Inventory turnover  rate}=\frac{\text{COGS}}{\text{Ending inventory}} $$

The forecast:
$$\text{Forcasted ending inventory} =\frac{\text{Forecasted COGS}}{\text{Inventory turnover  rate}} $$
---
We can add more sophistications to the forecast when the firm discloses more information:
- inventory turnover rates by product or category, specially important for diversified companies.
- launching of new products or stores: estimate the inventory should be added to the forecast

---
Step 2.4, estimate the company's expected _PPE_:

- _PPE_ is estimated as the prior year’s gross PP&E balance plus historical capital expenditures as a percentage of sales.

- Historical capital expenditures are obtained from the statement of cash flows.

- It is very common to subsequently adjusted forecasted PPE to examine the financial implications of higher (lower) levels of capital expenditures (sensitivity analyses)

---
Step 2.5, estimate expected accumulated depreciation:

Accumulated depreciation is estimated as the prior year’s accumulated depreciation balance plus forecasted depreciation (step 1.5).

Step 2.6, estimate the company's expected _net PP&E_:


---
Step 2.8, estimate the company's expected _accounts payable_:
$$\text{Accounts payable turnover rate}=\frac{\text{COGS}}{\text{Accounts payable balance}} $$

The forecast:
$$\text{Forcasted accounts payable} =\frac{\text{COGS}}{\text{Accounts payable turnover rate}} $$
---

Step 2.9, identify the _current portion of long-term debt_ from the footnotes of the financial statements.


Step 2.10, estimate expected _accrued expenses_:
- accrued expenses are usually estimated as a percentage of sales
- very basic intuition: if sales increase, the company will need to pay more salaries and recognize more operating expenses later on to match their revenues.
---
Step 2.11, estimate expected _tax payable_:
- what fraction of the tax expenses will be paid in the next year?
- we can estimate this fraction by looking at the historical trend in tax payable as a percentage of tax expenses

Step 2.13, estimate expected _other long-term liabilities_:
- if there is no reason to expect changes in the company's debt structure, we can assume that other long-term liabilities will be the same as the prior year's balance minus the expected current portion of long-term debt (step 2.9)
---

Step 2.16, estimate expected _retained earnings_:
$$\text{Forecasted retained earnings}=\text{Prior year’s retained earnings}+\text{Projected net income}-\text{Proyected dividends}$$

Step 2.17, estimated expected _cash_:
- Amount needed to balance total liability and equity with total assets
- crucual step: is further financing needed? can the company invest more in PP&E? can the company pay more dividends?
---
# 4. Sensitivity Analysis
---
# 4. Sensitivity Analysis
- We are assuming that many dimensions of the financials statements will change.
- Our approach is a good starting point to
  1. test the sheet and formula: there should not be drastic changes in the company's financial structure
  2. foresee how the company's financial structure will look if no significant changes happen in the future 
     1. valid for mature companies, 
     2. not so much for young or highly disruptive/distresed companies.
      
---
##  4.1 Univariate optimization
How much the company need to increase sales to meet EPS target?
  - is it feasible? if not, what else can be done?

Find the solution to the question: MS Excel: Data>What-if-Analysis>Goal Seeker.

Let's jump to the example in MS Excel.

---
## 4.2  Multivariate optimization
How much the company need to adjust its assumptions to meet  net income (or EPS) target?
  - sales growth rate
  - gross profit margin
  - SG&A, D&A
  - debt structure, and so on
  
Find the solution to the question: MS Excel: File>Options>Add-in> Solver

---
## 4.3 Sensitivity analysis  
Is the net income (or EPS) very sensitive to minor variations in the assumptions?

Find the solution to the question: MS Excel: Data>What-if-Analysis>Data Table.

---
## 4.4 Scenario analysis
Now we bunch assumptios together to create specific scenarios and ask:

- What if the company's assumptions are too optimistic or too pessimistic?

- What if next year the economy is in a recession as in 2008?
   
- What if the we have a pandemic as in 2020? or if we lose a major client?

We need to tailor or MS sheet  and bunch assumptions together to create each scenario.

---
# Based on:
- Subramanyam, K. R. (2014). Financial statement analysis. McGraw-Hill Education. Chapter 9.
- Fridson, M. S., & Alvarez, F. (2022). Financial statement analysis: a practitioner's guide. John Wiley & Sons. Chapter 12.

---
# Questions :question:
Check my website for an updated version of this presentation:

:point_right: [https://www.marceloortizm.com/](https://www.marceloortizm.com)
# Thanks :clap:
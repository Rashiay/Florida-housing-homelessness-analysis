# 📊 Florida Housing, Population Trends & Homelessness Group Analysis

An end-to-end Power BI business intelligence report examining the relationship between population growth, housing supply, housing affordability, and homelessness rates across Florida[cite: 1].

---

## 📌 Executive Summary

Florida's rapid population expansion has placed unprecedented pressure on its housing market[cite: 1]. This Power BI report integrates data from the **U.S. Census Bureau** and the **Annual U.S. Homeless Statistics Reports Database** to evaluate state housing trends from 2010 to 2023, featuring analytical projections through 2028[cite: 1].

### Key Insights
* **Population Growth vs. Housing Supply:** Florida’s population grew by over **3.5 million residents** from 2010 to 2023[cite: 1]. Year-over-year growth shows population growth frequently outpaces housing development, notably in 2015 and 2021[cite: 1].
* **Affordability Risk:** Sales of homes under **$300,000** have decreased sharply, restricting affordability[cite: 1]. Most sales occur in the $300,000–$399,999 range[cite: 1].
* **Homelessness & Vacancy Ratio:** The number of homeless individuals fluctuated from a high of 37,584 in 2011 to 12,502 in 2021, before rising to 22,925 in 2023[cite: 1]. A higher vacant housing-to-homeless ratio highlights untapped potential to address homelessness using existing housing stock[cite: 1].

---

## 🖼️ Dashboard Preview

| Overview Page | Housing & Income Trends |
| :---: | :---: |
| ![Dashboard Overview](assets/dashboard_overview.png) | ![Sales and Income](assets/sales_and_income.png) |

---

## 🛠️ Data Model & Key DAX Formulas

### 1. Homes Per 1,000 People
```dax
Homes Per 1,000 People = [Housing Units] / [Population] * 1000

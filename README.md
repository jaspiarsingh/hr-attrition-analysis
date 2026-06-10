# HR Attrition Analysis

## 📊 [View Live Dashboard](https://public.tableau.com/views/HrAttritionAnalysis_17811100713140/Dashboard1)

---

## Business Context

Employee attrition costs companies between 50–200% of an employee's annual salary in recruiting, onboarding, and lost productivity. For a company of 1,470 employees with a 16.1% attrition rate, that's a multi-million dollar problem hiding in plain sight.

> **The business question: Who is leaving, why, and who is next?**

This project analyzes IBM's HR dataset to surface the key drivers of attrition and identify current employees at the highest flight risk — giving HR leadership the data they need to act before it's too late.

---

## Key Findings

- **Sales Representatives have the highest attrition rate at 39.76%** — nearly 3x the company average, signaling a compensation or culture problem in the sales org
- **Overtime is the single biggest attrition driver** — employees who work overtime leave at a 30.53% rate vs 10.44% for those who don't, almost 3x higher
- **Low income + low satisfaction is a dangerous combination** — employees in the lowest income band with satisfaction score of 1 show 30%+ attrition rates
- **Young employees in early tenure are highest risk** — employees under 25 with 0-2 years at the company show a 49.23% attrition rate
- **Employees #2021 and #1131 are the highest flight risk** — both score 8/9 on the composite risk model based on overtime, satisfaction, income, tenure, and travel factors

---

## Recommendations

1. **Audit Sales Representative compensation** — a 40% attrition rate is unsustainable; benchmark salaries against market and introduce retention bonuses for top performers
2. **Implement an overtime monitoring policy** — flag employees logging consistent overtime for manager check-ins before burnout leads to resignation
3. **Create an early tenure retention program** — employees in their first 2 years are most at risk; structured mentorship and career pathing in this window would have the highest ROI
4. **Proactively engage the 20 flagged employees** — the flight risk scorecard identifies specific employees by ID; HR can cross-reference with managers for targeted retention conversations

---

## Dataset

**Source:** [IBM HR Analytics Employee Attrition Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset) — Kaggle  
**Size:** 1,470 employee records, 35 features  
**Type:** Synthetic but realistic HR data modeled on real attrition patterns  

---

## Tech Stack

| Tool | Purpose |
|---|---|
| MySQL | Data storage and analysis |
| Python (Pandas) | Data import and ETL |
| Tableau Public | Interactive dashboard |

---

## SQL Analysis

Five business-driven queries power the dashboard:

| Query | Business Question |
|---|---|
| Attrition by Department & Role | Which teams have the highest attrition rates? |
| Overtime vs Attrition | Does overtime drive employees to leave? |
| Compensation & Satisfaction | Are low earners and dissatisfied employees leaving more? |
| Tenure & Age Risk Bands | Which career stage is most at flight risk? |
| Flight Risk Scorecard | Which current employees show the most combined risk factors? |

Full queries available in the [`/sql`](/sql) folder.

---

## Project Structure

```
hr-attrition-analysis/
│
├── sql/
│   ├── 01_attrition_by_role.sql
│   ├── 02_overtime_attrition.sql
│   ├── 03_compensation_satisfaction.sql
│   ├── 04_tenure_age_risk.sql
│   └── 05_flight_risk_scorecard.sql
│
├── python/
│   └── import_hr.py
│
├── dashboard/
│   └── dashboard_screenshot.png
│
└── README.md
```

---

## Dashboard Preview

[![HR Attrition Dashboard](dashboard/dashboard_screenshot.png)](https://public.tableau.com/views/HrAttritionAnalysis_17811100713140/Dashboard1)

---

## Author

**Jaspiar Singh**  
Data Analyst | [linkedin.com/in/jaspiar](https://linkedin.com/in/jaspiar)

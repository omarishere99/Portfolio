# Telco Customer Churn Analysis

**Tools:** Power BI, DAX  
**Dataset:** 7,043 customers across 6 linked tables — [source data](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)  
**Live Dashboard:** [View on Power BI](#) ← replace with your published link

---

## Business Problem

A California-based telecommunications provider is losing 1 in 4 customers. Of 7,043 customers, 1,869 have churned — generating $1.53M in lost monthly revenue against a total charge base of $16.06M. With a large proportion of customers on flexible month-to-month contracts, the revenue base is structurally exposed to competitor pressure at any point in the customer lifecycle.

---

## Key Findings

- **Month-to-month customers churn at 42.71%** vs 2.83% on two-year contracts — a 15x gap making contract structure the single strongest retention lever
- **Fiber Optic customers churn at 40.72%** — the premium product is the most at-risk segment, with competitor speed and data offers as the top cited reasons
- **Senior citizens churn at 41.68%** vs 23.61% for non-seniors, accounting for $1.11M of lost monthly revenue
- **The top two churn reasons are competitor-driven** — a product competitiveness problem that retention campaigns alone cannot fix
- **San Diego accounts for $152K in lost monthly revenue** — disproportionate concentration pointing to a localised competitor or service issue

---

## Dashboard Pages

| Page | Business Question |
|------|------------------|
| Overview | How bad is the problem, what is driving it, and where is it most acute? |
| Demographics & Behaviour | Which customer profiles are churning and how does tenure affect retention? |
| Revenue Impact | Where is lost monthly revenue concentrated by segment, geography, and payment method? |

---

## Data Notes

- Dataset spans 6 linked tables joined on Customer ID. No data integrity issues identified.
- Lost monthly revenue ($1.53M) represents the sum of monthly charges for churned customers.
- Geographic analysis uses top N filter by churned customer count to avoid statistical noise from low-volume cities.
- Services matrix shows proportion of churned customers who had or did not have each service at the time of churn.

---

## Full Case Study

See [`telco_churn_case_study.docx`](./telco_churn_case_study.docx) for detailed findings and recommendations.

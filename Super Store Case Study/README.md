# Superstore Profitability Analysis

**Tools:** Power BI, DAX  
**Dataset:** 9,994 order lines, US retail, 2014–2017 — [source data](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)  
**Live Dashboard:** [View on Power BI](#) ← replace with your published link

---

## Business Problem

A US retail superstore generated $2.30M in sales across 2014–2017, with revenue growing from $484K to $733K. But underneath the growth, profit margin sits at just 12.5% and is being actively eroded by aggressive discounting, loss-making product sub-categories, and geographic markets where the business is selling at a loss. The business is growing revenue while undermining the profitability of that growth.

---

## Key Findings

- **Discounts above 30% generate negative profit margins** — orders with 51%+ discounts produce a -119.20% margin, meaning the business spends $2.19 to generate $1 of revenue on those transactions
- **Tables is an accelerating loss** — losses nearly tripled from ($3K) in 2014 to ($8K) in 2017; removing Tables and Bookcases would have added $9K to 2017 profit
- **Technology delivers 17.4% margin vs Furniture at 2.5%** — the product mix is working against profitability
- **Texas is the third largest state by sales but loses ($25.7K)** — five states are loss-making at scale despite significant sales volume
- **Machines: $189K in sales at 1.8% margin** — high revenue sub-category consuming operational resource for near-zero return

---

## Dashboard Pages

| Page | Business Question |
|------|------------------|
| Performance Overview | How is the business performing by year, region, state, and category? |
| Profitability Deep Dive | What is causing the margin problem — and what would profit look like if loss-making furniture lines were discontinued? |

Page 2 includes an interactive what-if slicer modelling the profit uplift from reducing Tables and Bookcases at different retention levels.

---

## Data Notes

- Discount Band and Discount Band Sort calculated columns created in Power BI to enable discount tier analysis.
- Adjusted Profit measure models the what-if scenario of reducing Tables and Bookcases retention — controlled via numeric slicer.
- Page 1 KPI cards reflect the selected year via slicer (defaulting to 2017).
- Recommendations are framed as investigations and structured interventions rather than immediate policy changes.

---

## Full Case Study

See [superstore_case_study.pdf](https://github.com/omarishere99/Portfolio/blob/main/Super%20Store%20Case%20Study/superstore_case_study.pdf) for detailed findings and recommendations.

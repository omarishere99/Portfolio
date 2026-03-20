# Uber NCR Ride Analytics 2024

**Tools:** Power BI, DAX  
**Dataset:** 150,000 ride bookings, NCR 2024 — [source data](https://www.kaggle.com/datasets/yashdevladdha/uber-ride-analytics-dashboard)  
**Live Dashboard:** [View on Power BI](https://app.powerbi.com/view?r=eyJrIjoiZWI3YmY3MjctODJhYi00NmM0LWFiMmItYjM2ZTU5YTU0NmY2IiwidCI6IjgyMTYwMGNjLWY1YzMtNDgxMC1hY2FkLWU2MWI4M2Q4YmE0ZiJ9&pageName=d32b4d2f4b0a122e7de3)

---

## Business Problem

Uber NCR completed only 62% of all ride bookings placed in 2024. The remaining 38% — 57,000 rides — were lost to driver cancellations, no driver availability, customer abandonment, or incomplete journeys. At an average fare of ₹508, this represents an estimated ₹28.97M in revenue the platform generated demand for but failed to convert.

---

## Key Findings

- **Driver cancellations account for 18% of all bookings** — but the true driver-fault figure is closer to 21% once misclassified customer cancellations are correctly attributed
- **Failure rate held flat at 38% across all 12 months** — structural, not seasonal
- **Vinobapuri (45.3%) and Akshardham (43.9%)** are the highest-failure pickup zones, sitting up to 7 points above the platform average
- **High failure zones and high volume zones are different problems** — requiring separate, targeted responses

---

## Dashboard Pages

| Page | Business Question |
|------|------------------|
| Overview | How is the business performing overall? |
| Ride Failures | Where are rides being lost and why? |
| Revenue | What does the financial picture look like by vehicle type, distance, and payment method? |

All pages include Vehicle Type, Pickup Location, and Month slicers for interactive drill-down.

---

## Data Notes

- A Booking ID recycling defect affecting 1,757 records was identified and resolved prior to import. Row count used as the booking grain throughout all measures.
- Revenue at risk figures are opportunity cost estimates based on average completed fare (₹508.30) applied to non-completed rides.
- Star schema model: central fact table with Date, Location, and Vehicle Type dimensions.

---

## Full Case Study

See [`uber_ncr_case_study.docx`](./uber_ncr_case_study.docx) for detailed findings and recommendations.

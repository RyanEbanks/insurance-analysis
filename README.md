# Analysis of 2025 Health Insurance Exchange Public Use Files

## Table of Contents
- [Project Background](#project-background)
- [Executive Summary](#executive-summary)
- [Insights Deep-Dive](#insights-deep-dive)
- [Recommendations](#recommendations)
- [Clarifying Questions, Assumptions, and Caveats](#clarifying-questions-assumptions-and-caveats)

## Project Background
The Centers for Medicare & Medicaid Services (CMS) Center for Consumer Information and Insurance Oversight (CCIIO) is committed to increasing transparency in the Health Insurance Exchanges. CMS publishes downloadable public use files (PUFs) so that researchers and other stakeholders can more easily access Exchange data. 

## Executive Summary
This analysis evaluates key indicators of health insurance market performance across the United States in 2025, focusing on premium costs, plan diversity, and issuer competitiveness.

## Insights Deep-Dive
### Sales Trends
* Olist averaged approximately R$15.8 million in annual sales over the past two years.
* São Paulo was consistently the top performing state, with sales decreasing the further away from the countries economic hub.
* Sales show clear seasonality, with Spring peaking in total sales. However some months in 2024 are missing, introducing potential bias.
<img width="952" height="528" alt="Sales By Months and Year" src="https://github.com/user-attachments/assets/e04a9e28-2b96-43a3-8b2b-5f9559506320" />
<img width="1196" height="866" alt="Sales  By State" src="https://github.com/user-attachments/assets/7ab66dc8-0a81-418d-90ff-3eea0701c068" />
<img width="951" height="838" alt="Sales  From Highest to Lowest" src="https://github.com/user-attachments/assets/9897164d-0678-4c2e-9b37-70cc5167dc06" />

### Growth Rates
* São Paulo had the highest overall state level growth at 37.47% over the two years.
* Spring had the highest seasonal growth rate, contributing approximately R$1.8 million across both years.
* May stood out as a consistent month of high growth yearly with a growth rate of 100.22%.
<img width="272" height="85" alt="state growth rate" src="https://github.com/user-attachments/assets/a8ed2b00-5901-458a-9b04-2ae9d03f5286" />
<img width="952" height="852" alt="Growth Rate  Monthly   Yearly" src="https://github.com/user-attachments/assets/35476d11-695e-4c23-93f4-1c8173b3ae50" />
<img width="264" height="85" alt="Top Month" src="https://github.com/user-attachments/assets/e69309b8-f367-40d3-a283-15e14d1bbe65" />

### Refund Rates
* Summer recorded the highest seasonal refund rate at 0.90%, though remains within acceptabel bounds.
* The sate with the highest refund rate was Rondônia, likely due to the its geographical distance from the main state.
* In 2023, the peak refund month was March at 1.59%, whereas in 2024 July had the highest rate at 1.81%.
<img width="570" height="87" alt="Refunds" src="https://github.com/user-attachments/assets/5b736b92-56cd-4d4b-8e12-af58ee4a1951" />
<img width="908" height="838" alt="Refund Rate  By Months" src="https://github.com/user-attachments/assets/056596f8-9061-4f9d-a6b6-984b01c9d1b7" />

## Recommendations
### Maximizing Sales and Growth Rates
* __Expand Beyond São Paulo:__ São Paulo dominates sales, perfomance drops in states farther from this hub. Increasing outreach, promotions, and logistics support in underperforming states can unlock new markets.
* __Capitalize on Seasonal Opportunities:__ While spring leads in sales, other seasons including summer, fall and christmas offer untapped revenue. Launching seasonal compaigns and promotions during those times can incentivise growth.
* __Boost Repeat Purchases with Loyalty Programs:__ Introducing seasonal themed events, rewards and loyalty programs can encourage customers to buy multiple of the same items. This could strengthen customer retention and average oder value.

### Maintaining Low Refund Rates
* __Replicate Effective Practices:__ Identify what worked during the months with low refund and apply those practices across the board, including product quality checks and better delivery communication.
* __Analyze Refund Patterns by State:__ Conduct a deeper analysis into which products and categories are most refunded in each state. This will help tailer better solutions whether its product sourcing or customer service interventions based on regional trends.

## Clarifying Questions, Assumptions, and Caveats
### Questions for Stakeholder Prior to Project Advancement
* Which statuses actually represent a completed payment?
  * Is "unavailable" a finalized status that should be treated as paid?
  * Does "created" mean the order was never finalized?
* Transactions with R$0 were assumed to not be valid.

### Assumptions and Caveats
* Orders with status ```delivered```, ```invoiced```, ```processing```, ```approved```, ```shipped```, and ```unavailable``` were assumed to be paid orders.
* Orders with status ```canceled``` were categorized as cancelled, and ```created``` as never paid.
<img width="200" height="214" alt="image" src="https://github.com/user-attachments/assets/b20322bb-9bdf-40a2-beeb-8cdccb3dbd72" />

* R$0 Transactions were kept in the dataset but filtered out when creating the charts.
---
* See the raw data and my cleaning, and pivot tables in the [Excel Workbook]([Uploading Insurance_v2025.1.twb…]()
).
* [See my SQL Queries in the SQL file](./exploration/olist_exploration.sql).
* [Go to Data Cleaning Notes](./exploration/data%20cleaning/cleaning.md).
* [Tableau Dashboard](./exploration/Olist.twbx).


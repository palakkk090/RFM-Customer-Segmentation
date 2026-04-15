# RFM Customer Segmentation Analysis — Online Retail

## Objective
Segment 5,878 customers of a UK-based online retail store into 
behavioral groups using RFM (Recency, Frequency, Monetary) analysis 
to identify high-value customers, flag at-risk segments, and 
recommend targeted marketing strategies.

## Dataset
- Source: Kaggle dataset- Online Retail II
- Period: December 2009 – December 2011
- Size:1,067,371 transactions across 43 countries
- Products:5,305 unique SKUs
- Primary Market: United Kingdom (92% of transactions)
- Link:[Online Retail II Dataset - Kaggle](https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci)

## Tools Used
- Python — Pandas, NumPy, Matplotlib, Seaborn
- Jupyter Notebook — end-to-end analysis walkthrough
- Microsoft Excel — interactive dashboard

##  Process
1. Data Cleaning — removed null CustomerIDs, cancelled orders 
   (invoices starting with 'C'), negative quantities and prices
2. Feature Engineering — calculated Revenue column 
   (Quantity × Price)
3. RFM Calculation — computed Recency, Frequency, and Monetary 
   value per customer using reference date
4. Scoring — assigned 1–5 scores per RFM metric using quantile 
   binning
5. Segmentation — classified customers into 6 behavioral groups 
   based on combined RFM scores
6. Visualization — built charts and Excel dashboard for 
   business reporting

##  Key Findings

- Champions (1,300 customers) drive 68.35% of total revenue 
  despite being only 22% of the customer base
- 824 At-Risk customers haven't purchased in 369 days on average 
  — representing £1.6M in recoverable revenue
- 1,275 Lost customers last purchased 468 days ago on average 
  with very low avg spend of £256
- Loyal Customers are the largest segment (1,403) with strong 
  upsell potential at £1,934 avg spend

## Business Recommendations

Champions - Loyalty rewards, early product access 
Loyal Customers - Upsell premium products, ask for reviews 
At Risk - Win-back campaigns, limited-time discounts 
Potential Loyalists - Membership offers, personalized nudges 
New Customers - Onboarding journey, first purchase incentives 
Lost - Aggressive re-engagement or deprioritize spend 

## Files
- RFM_Analysis.ipynb — Full Python code and analysis
- Segment_Summary.xlsx — Summary table with Excel dashboard
- RFM_Segments.xlsx — Complete customer-level RFM data
- segment_distribution.png — Customer count by segment
- revenue_by_segment.png — Revenue breakdown chart
- rfm_heatmap.png — RFM values heatmap
- revenue_pie.png — Revenue contribution pie chart

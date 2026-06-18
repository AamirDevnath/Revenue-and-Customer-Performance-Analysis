# Revenue-and-Customer-Performance-Analysis
End-to-end data analysis of a transactional dataset from a UK-based online retailer. The analysis was structured around five business questions a commercial analytics team would be expected to answer ahead of a board strategy review, covering product performance, revenue trends, customer concentration, geographic markets, and data quality.

This project was also a deliberate learning exercise in Python for data analysis, working through core concepts in pandas, numpy, and matplotlib from first principles.

### Business Questions

The analysis was structured around five questions:

- Which products drive the most revenue, and which are underperforming?
- How does revenue trend month-on-month, and are there seasonal patterns?
- Are we over-reliant on a small number of high-value customers?
- Which countries are our biggest markets, and where is growth or decline occurring?
- Are the underlying numbers trustworthy before board presentation?

### Analytical Workflow

The project followed a structured eight-step data analysis workflow:

- Define business objectives
- Load and inspect data
- Clean and validate data
- Univariate analysis
- Bivariate analysis
- Answer business questions
- Summarise findings
- Recommendations

### Answers

- Q1 
A small number of products generate the vast majority of revenue. A Pareto chart was used to identify the exact crossover point where a fraction of the catalogue accounts for 80% of total revenue. The bottom-performing products (filtered to those with at least 10 transactions to exclude noise) were identified as candidates for ranging review, repricing, or discontinuation.


- Q2 
Revenue shows a clear seasonal pattern with a peak in the fourth quarter (October–November), consistent across years. This has direct implications for inventory planning, staffing, and marketing campaign timing. Month-on-month percentage change was calculated and visualised alongside the absolute trend, separating the question of how big a month was from whether it was growing or declining.


- Q3 
A Lorenz curve confirmed significant customer revenue concentration — a minority of customers account for the majority of revenue, representing a retention risk. RFM (Recency, Frequency, Monetary) analysis was applied to score every customer across three behavioural dimensions and assign each to one of five segments: Champions, Loyal Customers, Potential Loyalists, At Risk, and Lost.
The Champions segment, despite being small in headcount, contributes disproportionately to total revenue. The At Risk segment represents the highest priority for a re-engagement campaign.


- Q4
The UK dominates revenue. International markets were analysed separately to avoid the UK obscuring all other bars on a shared scale.
A period-on-period comparison (splitting the dataset into two halves) was used to calculate growth and decline rates by country, separating market size from market momentum — a distinction that is critical for international investment decisions.


- Q5
A significant limitation is the null Customer ID rate, which restricts full coverage of customer-level analysis. This should be addressed at the point-of-sale data capture stage before the next reporting cycle.

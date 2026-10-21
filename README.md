# Retail Analytics: DataMelon Labs Industry Fellowship

End-to-end retail analytics project built during the **DataMelon Labs Industry Fellowship (2026)**. Five connected analyses on a single retail dataset, taking leadership from a high-level performance view down to geography, department, and customer-level insights.

**Author:** Kartikey Singh | **Role:** Data Analyst
**Tools:** Databricks | SQL | Power BI
**Fellowship period:** August 2026 - October 2026

---

## Business Context

Leadership needed to understand what was driving retail sales growth, whether that growth was comparable year over year, where it was coming from geographically and across products, and whether a growing customer base was translating into stronger customer value.

## Analytical Flow

Business Performance → LFL Growth → Geography → Products and Departments → Customers

## Projects

| # | Project | Focus | Folder |
|---|---------|-------|--------|
| 1 | **Retail Business Performance Deep-Dive** | 12-month rolling analysis of sales, loyalty, regions, categories, payments, acquisition, and spend per customer | 01_business_performance |
| 2 | **Like-for-Like (LFL) Performance Analysis** | 2026 vs 2025 growth using matched trading days, built in Databricks SQL | 02_lfl_performance |
| 3 | **Geography Deep Dive** | Regions, cities, city tiers, store formats, revenue concentration, underperforming markets | 03_geography_deep_dive |
| 4 | **Department Deep Dive** | Department concentration, category growth, customer segments, seasonality, brands, engagement | 04_department_deep_dive |
| 5 | **Customer Analysis** | Customer growth, new vs repeat, loyalty sales, spend per customer, age groups, regions | 05_customer_analysis |

---

## 1. Retail Business Performance Deep-Dive (12-Month Rolling)

**Objective:** Understand the drivers behind overall sales growth rather than relying only on total sales.

| Metric | Result |
|--------|--------|
| Total sales | INR 895.3M |
| Recent growth | 7.7% over the last 6 months |
| Loyalty program sales | INR 497.3M (55% of total sales), growing faster than the overall business |
| Regional contribution | North 26.5%, Central 13.9% |
| Category concentration | 16 product categories contribute 80% of sales |
| Payment mix | Card and UPI together account for 93% of transactions |
| Customer acquisition | Up 23.8% over the last 6 months |
| Spend per customer | Down 13% over the last 6 months |

**Interpretation:** Sales growth was supported strongly by customer-base expansion, while individual customer spending declined.

## 2. Like-for-Like (LFL) Performance Analysis

**Objective:** Create a comparable year-over-year view by matching trading days rather than calendar dates. Implemented in Databricks SQL with Gold-layer tables for Current Year, Previous Year, and LFL comparison.

| Area | Result |
|------|--------|
| Overall LFL sales growth | +19.33% |
| Transaction growth | +20.90% |
| Regions | West +21.68%, with all regions showing double-digit growth |
| Cities | Nagpur +27.13%, Noida +26.14% |
| Departments | Household +32.38%, core categories around 18-20% |
| Monthly trend | 18-22% range, no significant seasonality observed |

**Interpretation:** Growth was broad-based across regions, cities, departments, and months rather than concentrated in a single area.

## 3. Geography Deep Dive

**Objective:** Understand whether growth was broad-based geographically, which locations and formats performed strongly, and where underperformance existed.

| Area | Result |
|------|--------|
| Market growth | No declining markets; 20-26% YoY across all five regions |
| Strongest regions | West and South at 25%+ |
| City tiers | Tier 1 27.7%, Tier 2 22.7%, Tier 3 17.2% |
| Formats | Fresh 28-32%; Express 15-20% vs 25-30% for Fresh and Supermarket |
| Revenue concentration | Top 5 cities 39%, top 15 cities 86% of revenue |
| Underperformers | Jabalpur, Raipur, Dehradun at 11-17% growth (Tier 3 Express) |
| New customers | 55-65% growth across analyzed markets |

**Interpretation:** The findings support a differentiated geographic strategy and make monitoring of major cities important because of revenue concentration.

## 4. Department Deep Dive

**Objective:** Identify high-performing and underperforming parts of the product portfolio and understand customer, regional, and format differences.

| Area | Result |
|------|--------|
| Concentration | Top 5 departments drove 60-70% of total business |
| Growth categories | 30-50%+ YoY growth |
| Customer value | Repeat customers 3-5x more valuable than one-time customers |
| Seasonality | October-November festival periods showed about 30-40% uplift |
| Brands | Leaders held 40-60% share in analyzed categories |
| Repeat rate | 30-90% across the analyzed engagement view |
| Hypermarket trips | 12-15 items, INR 1,200-1,500 baskets |
| Supermarket trips | 5-8 items, INR 400-600 baskets |

**Interpretation:** The analysis gives a framework for balancing traffic-driving and margin-generating categories, tailoring assortment by region and format, and planning around seasonality.

## 5. Customer Analysis

**Objective:** Understand whether customer growth was translating into stronger customer value and how behavior differed across age groups and regions.

| Area | Result |
|------|--------|
| Customers | 13,944 current-year customers, +60.6% YoY |
| New customers | 2,453, equal to 17.6% of the customer base |
| Repeat rate | 96.9%, down 0.4 percentage points |
| Loyalty sales | INR 214.74M, up 48.7% YoY |
| Spend per customer | INR 15,401, down 7.4% YoY |
| Age 26-35 | Largest group: 2,120 customers (30%), INR 18,621 spend per customer |
| Age 36-45 | INR 20,497 spend per customer, 16.23 transactions per customer, spend up 2.6% |
| Age 60+ | INR 17,767 spend per customer, up 3.3% |
| Regional customers | West 3,580 (+64.7%), South 2,826 (+59.8%), North 2,818 (+61.4%) |
| Regional spend per customer | North INR 15,960, Central 15,889, West 15,702, East 15,377, South 13,472 |

**Interpretation:** The customer base expanded strongly while spend per customer declined, so customer-value analysis remains important.

---

## Overall Conclusion

The combined analysis shows strong business and customer-base growth across the evaluated views. It also highlights that growth in customer numbers does not necessarily translate into higher spend per customer. Together, the projects provide a structured basis for deeper customer-value, geographic, and product-performance analysis.

## Repository Structure

```
├── README.md
├── 01_business_performance/
├── 02_lfl_performance/
├── 03_geography_deep_dive/
├── 04_department_deep_dive/
├── 05_customer_analysis/
└── reports/
    └── Industry_Project_Report.pdf
```

Each project folder contains its own README, the dashboard exported as PDF, and the Power BI file where included.

## Tech Stack

| Tool | Used for |
|------|----------|
| Databricks | Data processing and Gold-layer tables |
| SQL | Querying, trading-day matching, LFL calculations |
| Power BI | Dashboards and visualization |

## Skills Demonstrated

- SQL and Databricks (Gold-layer tables, trading-day matching)
- Like-for-like and year-over-year growth analysis
- Geographic, product, and customer segmentation
- KPI design and Power BI dashboard development
- Translating analysis into business interpretation

## Data Note

The dataset was provided by DataMelon Labs as part of the fellowship and is used here for portfolio purposes.

## Author

**Kartikey Singh**, Data Analyst

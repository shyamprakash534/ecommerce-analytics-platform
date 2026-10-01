# E-Commerce Sales, Customer & Profitability Analytics Platform

Portfolio-grade analytics dashboard for interactive e-commerce performance analysis.

The project is designed to show how raw transactional-style data can be transformed into business-facing views for **sales, profitability, customers, products and regional performance**.

## Live Application

**https://ecommerce-analytics-platform-b342.onrender.com**

## What It Demonstrates

- Building an interactive analytics application in Python
- Translating business questions into measurable KPIs
- Customer, product and regional analysis
- Profitability and discount diagnostics
- Reproducible synthetic data generation
- Interactive filtering and visual exploration

## Dashboard Sections

### Executive Overview
High-level revenue, profit, margin and order KPIs for quickly understanding overall performance.

### Sales & Profitability
Revenue, profit, margin and discount analysis across the selected period.

### Customer Analytics
Customer segmentation, spend patterns and customer-level performance analysis.

### Product & Category
Product and category contribution, revenue and profitability diagnostics.

### Regional Performance
Regional comparison using revenue, profit and related performance measures.

## Key Features

- Executive Overview
- Sales & Profitability
- Customer Analytics
- Product & Category
- Regional Performance
- Region, category, segment and date filters
- Revenue, profit, margin, discount and leakage KPIs
- Customer segmentation and spend analysis
- Product and regional profitability diagnostics

## Data & Reproducibility

The dashboard generates a deterministic synthetic e-commerce dataset using **NumPy seed 42** when started from a clean checkout.

This makes the project easier to review because the same starting conditions can be reproduced without relying on a private production dataset.

The data is intended for analytics demonstration rather than representing a real company's customers, transactions or financial performance.

## Architecture

```text
Synthetic E-Commerce Data
          |
          v
     Pandas / NumPy
          |
          v
   Analytics Calculations
          |
          v
      Plotly Charts
          |
          v
    Streamlit Dashboard
```

## Stack

| Area | Technology |
| --- | --- |
| Language | Python |
| Data processing | Pandas, NumPy |
| Visualization | Plotly |
| Dashboard | Streamlit |
| Deployment | Render |

## Run Locally

```bash
git clone https://github.com/shyamprakash534/ecommerce-analytics-platform.git
cd ecommerce-analytics-platform

python -m venv .venv

# Windows
.venv\Scripts\activate

# Linux/macOS
source .venv/bin/activate

pip install -r requirements.txt
streamlit run app.py
```

Open the local URL printed by Streamlit.

## Engineering Notes

The application prioritizes **clarity and reproducibility over infrastructure complexity**. A deterministic local dataset means reviewers can run the dashboard without credentials, external databases or a private data source.

For a production analytics platform, additional concerns would include:

- Data warehouse or lakehouse integration
- Data quality monitoring
- Access control and governance
- Incremental data ingestion
- Automated testing of business metrics
- Observability and cost monitoring

## Limitations

- The dataset is synthetic and should not be interpreted as real business performance.
- Dashboard results depend on the generated dataset and implemented KPI definitions.
- The project demonstrates an analytics application rather than a complete production data platform.

## Author

**Shyam Prakash**

- GitHub: https://github.com/shyamprakash534
- LinkedIn: https://www.linkedin.com/in/shyam-prakash-vemula-721029263

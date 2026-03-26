# project-4-supply-chain-performance

Project 4 — Supply Chain Performance & Risk Analytics
📌 Overview
This project analyzes end‑to‑end supply chain performance using a dataset containing logistics, manufacturing, supplier, cost, revenue, and risk indicators. The goal is to identify operational bottlenecks, quantify risk exposure, and uncover cost‑to‑profit relationships across carriers, suppliers, transport modes, and product categories.

The project demonstrates a full analytics workflow using SQL (BigQuery) and Tableau, supported by clear documentation and a professional GitHub structure.
------------------------------------------
project-4-supply-chain-performance/
│
├── sql/
│   ├── cleaning.sql
│   ├── feature_engineering.sql
│   └── analysis_pack.sql
│
├── docs/
│   ├── project_overview.md
│   ├── methodology.md
│   ├── insights_summary.md
│   └── screenshots/
│       └── dashboard_full.pdf
│
└── README.md
-----------------------------------------------------------
🧠 Key Objectives
Clean and standardize raw supply chain data

Engineer new performance and risk metrics

Analyze cost drivers and profit margins

Evaluate supplier and carrier performance

Identify high‑risk SKUs and routes

Build a Tableau dashboard for executive insights

Document the full workflow for portfolio presentation

🛠 Tools & Technologies
BigQuery — SQL cleaning, transformation, feature engineering

Tableau — dashboard visualization

GitHub — version control and documentation

📊 Dashboard
A Tableau dashboard was created to visualize:

Cost structure

Profitability

Supplier performance

Logistics efficiency

Risk indicators

A PDF export is included in: docs/screenshots/dashboard_full.pdf
------------------------------------------------

🧹 SQL Pipeline
1. Cleaning Layer
cleaning.sql standardizes:

Categorical fields (trim, casing, normalization)

Numeric fields (FLOAT64 casting, non‑negative enforcement)

Supplier, carrier, and route labels

Output table: supply_chain_cleaned_p4
---------------------------------------------
2. Feature Engineering Layer
feature_engineering.sql creates:

Logistics efficiency tiers

Manufacturing performance tiers

Cost‑to‑revenue ratios

Profitability classifications

Supplier and transport risk tiers

Composite supply chain risk index

Output table:supply_chain_engineered_p4
---------------------------------------------------
3. Analysis Layer
analysis_pack.sql includes structured analysis for:

Cost breakdown

Profitability patterns

Supplier reliability

Logistics performance

Risk segmentation

These queries support the dashboard and insights summary.

📈 Key Insights
Highlights from the analysis (full details in insights_summary.md):

Logistics and manufacturing cost are the largest contributors to total cost

Profit margins vary widely across SKUs due to inconsistent cost structures

Supplier lead time is a major bottleneck affecting production and fulfillment

Transport mode strongly impacts cost and lead time

High defect rates correlate with high supplier risk and lower profitability

Certain routes consistently show higher delays and cost overruns

Stock level variability directly affects revenue and demand fulfillment

📘 Documentation
All project documentation is stored in /docs:

project_overview.md — high‑level summary

methodology.md — full workflow explanation

insights_summary.md — key findings and business implications

🏁 Conclusion
This project demonstrates a complete, end‑to‑end supply chain analytics workflow. It highlights your ability to:

Clean and structure complex operational data

Engineer meaningful performance and risk metrics

Build analytical models

Communicate insights through dashboards and documentation

-------------------------------------------

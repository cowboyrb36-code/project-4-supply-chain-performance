Methodology — Supply Chain Performance & Risk Analytics
1. Overview of the Analytical Workflow
This project follows a structured, industry‑standard analytics workflow designed to mirror real supply chain analytics practices. The workflow includes:

Data ingestion

Data cleaning & standardization

Feature engineering

Exploratory analysis

Performance & risk modeling

Dashboard development

Documentation & insights synthesis

Each step is executed using SQL in BigQuery and visualized through Tableau.
--------------------------------------
2. Data Ingestion
The dataset was loaded into BigQuery under:
my-healthcare-project-487800.Supply_chain_data_project4.Supply_chain_features_project4
------------------------------------

The raw dataset includes:

Logistics metrics

Manufacturing metrics

Supplier performance

Cost & revenue fields

Risk indicators

Customer & product attributes

This provides a complete view of the supply chain lifecycle.

---------------------------------
3. Data Cleaning
A dedicated cleaning script (cleaning.sql) was created to:

Normalize categorical fields (trim, casing, formatting)

Convert all numeric fields to FLOAT64

Enforce non‑negative values for cost, time, and volume metrics

Standardize naming conventions

Remove inconsistencies in supplier, carrier, and route labels

The cleaned dataset was saved as:supply_chain_cleaned_p4
------------------------------------------------------------

4. Feature Engineering
Feature engineering is essential for transforming raw operational data into actionable insights.
The engineered dataset (created in feature_engineering.sql) includes:

4.1 Performance Metrics
Logistics Efficiency Tier

Manufacturing Performance Tier

Cost‑to‑Revenue Ratio

Profit per Unit

Lead Time Variance

4.2 Risk Metrics
Supplier Risk Tier

Transport Mode Risk

Route Risk Score

Composite Supply Chain Risk Index

4.3 Inventory & Demand Metrics
Stock Risk Flag

Demand‑to‑Supply Ratio

SKU Profitability Classification

These engineered fields enable deeper analysis and more meaningful dashboard visuals.

5. Exploratory Analysis
The analysis pack (analysis_pack.sql) includes:

5.1 Cost Analysis
Total cost breakdown

Logistics vs manufacturing cost contribution

High‑cost SKUs and suppliers

5.2 Profitability Analysis
Profit margin distribution

Profit per unit

High‑profit vs low‑profit SKUs

5.3 Supplier Performance
Lead time reliability

Supplier risk segmentation

Supplier contribution to defects

5.4 Logistics Performance
Carrier efficiency

Transport mode comparison

Route‑level delays and cost patterns

5.5 Risk Analysis
High‑risk SKUs

High‑risk suppliers

Correlation between risk and cost

6. Dashboard Development
A Tableau dashboard was built using the original dataset to visualize:

Cost structure

Profitability

Supplier performance

Logistics efficiency

Risk indicators

The dashboard PDF is stored in: docs/screenshots/
-----------------------------------------

7. Documentation & Reporting
The project includes:

project_overview.md — high‑level summary

methodology.md — this document

insights_summary.md — key findings and business implications

README.md — main project landing page

This ensures the project is fully transparent, reproducible, and portfolio‑ready.

8. Conclusion
This methodology demonstrates a complete, end‑to‑end supply chain analytics workflow using SQL, BigQuery, and Tableau. The project highlights your ability to:

Clean and structure complex operational data

Engineer meaningful performance and risk metrics

Build analytical models

Communicate insights through dashboards and documentation



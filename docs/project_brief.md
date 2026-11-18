
# Project Brief – Sales Analytics Project

## 1. Business Scenario

Olist is a Brazilian e-commerce marketplace connecting customers and sellers across multiple product categories and geographic regions.

This project simulates an analytics engagement for a hypothetical e-commerce client using historical Olist marketplace data.

The client has defined 14 analytical requirements covering commercial performance, customer behavior, product performance, payments, fulfillment, and seller activity.

The project is a portfolio case study rather than a commissioned engagement with Olist.

## 2. Problem Statement

The source data is distributed across nine datasets containing transactional, customer, product, seller, payment, delivery, and review information.

Direct analysis is complicated by inconsistent geographic text, repeated records, missing values, differing data granularities, and relationships between transactional entities.

The project requires preparation and integration of these datasets, followed by analytical modeling and reporting to address the defined business requirements.

## 3. Objectives

- Assess the structure, quality, and analytical suitability of the source data.
- Prepare and integrate relevant datasets while preserving the original source files.
- Develop an analytical model supporting the defined business requirements.
- Calculate sales, customer, product, fulfillment, and seller performance metrics.
- Develop a Power BI report for communicating analytical results.
- Document transformation decisions, assumptions, limitations, and findings.

## 4. Stakeholders

The following stakeholder groups are assumed for the hypothetical business scenario.

| Stakeholder | Analytical Interest |
|---|---|
| Business Management | Overall sales and commercial performance |
| Sales and Marketing | Customer behavior, product demand, pricing, and promotions |
| Product and Category Management | Category contribution, recent products, seasonality, and product associations |
| Operations and Logistics | Delivery performance and fulfillment efficiency |
| Customer Experience | Customer reviews and delivery satisfaction |
| Seller Management | Seller performance and local-market opportunities |
| Finance | Payment distribution and hypothetical profitability |

## 5. Data Sources

The project uses the Olist Brazilian E-Commerce Public Dataset.

The dataset consists of nine CSV files containing:

- Customers
- Geolocation
- Orders
- Order items
- Order payments
- Products
- Sellers
- Product category translations
- Order reviews

Raw order purchase timestamps cover September 2016 to October 2018.

Following preparation and consolidation, six processed datasets support the Power BI analysis.

Detailed source schemas, processed schemas, field definitions, and logical relationships are documented in the [Data Dictionary](data_dictionary.md).

## 6. Project Scope

### 6.1. Analytical Scope

| Business Domain | Requirements |
|---|---|
| Executive sales overview | BR-01 |
| Product and category performance | BR-02, BR-04, BR-05, BR-06, BR-07, BR-08, BR-13 |
| Customer retention and payments | BR-03, BR-10 |
| Promotion and profitability | BR-09 |
| Fulfillment and customer experience | BR-11, BR-12 |
| Seller and local-market performance | BR-14 |

The complete analytical questions and acceptance requirements are defined in [Business Requirements](business_requirements.md).

### 6.2. Technical Scope

- Source-data storage in Microsoft SQL Server.
- Database creation and schema inspection using SQL.
- Data retrieval, assessment, cleaning, and transformation using Python.
- Processed CSV dataset generation.
- Analytical modeling and calculations using Power BI and DAX.
- Interactive reporting and project documentation.
- Version control using Git.

### 6.3. Out of Scope

- Production deployment and automated data refresh infrastructure.
- Predictive modeling and machine learning.
- Real-time business monitoring.
- Actual promotion execution and experimental validation.
- Verified profitability analysis using actual product costs.
- Causal inference regarding sales, pricing, or customer behavior.

The project focuses on descriptive, comparative, and scenario-based analytics.

## 7. Assumptions and Constraints

| Area | Assumption or Constraint |
|---|---|
| Business context | The client and stakeholder groups are hypothetical. |
| Source preservation | Original source files remain unchanged; transformations are applied to derived datasets. |
| Reporting period | Analysis is based on historical records and relevant dataset-relative dates. |
| Sales | The implemented sales measure uses aggregated item prices excluding freight. |
| Customers | The current processed model uses customer-record identifiers rather than persistent customer identifiers. |
| Product launch | First observed purchase date is used as a proxy for launch date. |
| Profitability | The BOGO scenario assumes a 40% original profit margin because actual cost information is unavailable. |
| Transaction grain | The processed orders table contains aggregated transaction groups rather than unique orders. |
| Data coverage | Timestamp conditions and inner joins restrict the transactions available for analysis. |
| Financial accuracy | Item and payment aggregates require reconciliation before final business interpretation. |

## 8. Deliverables

| Deliverable | Location | Status |
|---|---|---|
| Project overview and execution instructions | `README.md` | Documented |
| Business requirements | `docs/business_requirements.md` | Documented |
| Project definition | `docs/project_brief.md` | Documented |
| Source and processed data dictionary | `docs/data_dictionary.md` | Documented |
| Database setup and metadata queries | `sql/01_create_db.sql` | Implemented |
| Data assessment and preparation notebook | `notebooks/01_data_cleaning.ipynb` | Implemented |
| Python transformation script | `src/data_cleaning.py` | Implemented |
| Six processed datasets | `data/processed/` | Generated |
| Power BI report | `powerbi/sales_dashboard.pbix` | 14 report pages implemented; validation outstanding |
| Findings and limitations | `docs/findings.md` | Data preparation findings documented; final business results outstanding |

## 9. Acceptance Criteria

The project should be considered analytically complete when:

- Data transformations are documented and reproducible.
- Table relationships and aggregation granularities are validated.
- Financial and quantity totals are reconciled.
- Each of the 14 business requirements is addressed using appropriate calculations and visuals.
- Assumptions and analytical limitations are explicitly documented.
- Reported findings are traceable to validated analytical results.

The current implementation establishes the data preparation workflow and report structure. Full analytical acceptance remains dependent on calculation validation and reconciliation.

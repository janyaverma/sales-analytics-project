# Sales Analytics Project

This is a data analytics project. For the lifecycle and process of completing this project I have taken inspiration from the CRISP-DM framework used in the tech industry. Although it was developed for data mining, it is also useful as a general framework for analytics projects.  

## 1. Problem Definition

Here I will define the business problem and questions that are required to be answered.

### 1.1. Business context

### 1.2. Objectives 

### 1.3. Stakeholders

### 1.4. Analytical Questions

The project addresses 14 analytical questions
defined by a hypothetical e-commerce client.

These requirements guide the development of
the Power BI dashboard, covering key business
areas such as sales performance, customer
behavior, and product performance.

For the complete list of analytical requirements,
see [Business Requirements](docs/business_requirements.md).

## 2. Tech Stack

I have used the following tools for doing this project.

### 2.1. Python
#### 2.1.1. Numpy
#### 2.1.2. Pandas

### 2.2. MS SQL

### 2.3. PowerBI

## 3. Data Understanding

### 3.1. The data source and its license and access conditions.

### 3.2. The schema, meaning, and quality of data.

### 3.3. Data dictionary

## 4. Data Quality Assessment And Preparation

Here I have talked about the cleaning and preparation of the data that include but is not limited to the following:

### 4.1. Filter and join

### 4.2. Missing values

### 4.3. Duplicates and inconsistent records

### 4.4. Data types

## 5. Data Transformation And Analysis

For analytics I have used the following:

### 5.1. Exploratory data analysis

### 5.2. SQL queries

### 5.3. Python analysis

### 5.4. KPI calculations

## 6. Visualization and communication

### 6.1. Power BI data model

### 6.2. Measures 

### 6.3. Dashboard 

### 6.4. Findings

## 7. Validation and review

Here I will verify calculations and assess whether the results answer your original questions. 

### 7.1. Reconciliation of totals

### 7.2. Calculation tests

### 7.3. Conclusions verification

## 8. Delivery And Documentation

The deliverables for this project include the powerbi reports and dashboard and the reproducible python and sql results.


The process is iterative. If a SQL result reveals a data-quality issue, return to data preparation; if a dashboard exposes an ambiguous KPI, revisit its definition.

---

## Skills Demonstrated

This project is designed to demonstrate three core competencies relevant to data analytics.

### 1. Analytical Thinking
- Translate a business problem into specific, answerable analytical questions.
- Define relevant KPIs and explain their significance.
- Interpret results in the context of the original business problem.
- Develop evidence-based findings and recommendations.

### 2. Technical Competence
- Use SQL to query, join, aggregate, and validate data.
- Use Python for data preparation, exploratory analysis, and additional validation.
- Build an interactive Power BI dashboard to communicate results.
- Check the consistency and correctness of key metrics across the analytical workflow.

### 3. Professional Working Practices
- Organize code, data, documentation, and deliverables in a clear project structure.
- Document data sources, assumptions, metric definitions, and limitations.
- Make the analytical workflow understandable and reproducible, where the available data and tools permit.
- Present findings clearly and support conclusions with evidence.
- Practice version control and commit meaningful changes throughout the project instead of uploading everything at the end. Use clear messages such as 'Add sales KPI queries'.

---

# Project Structure

## Directory structure is as follows:

```text
sales-analytics-project/
│
├── README.md
├── .gitignore
├── .gitattributes
├── requirements.txt
├── docs/
│   ├── project_brief.md
│   ├── data_dictionary.md
│   ├── business_requirements.md 
|   └── findings.md
│ 
├── data/
│   ├── raw/
│   └── processed/
│
├── sql/
│   ├── 01_create_db.sql
|
│
├── notebooks/
|   ├── 01_data_cleaning.ipynb
│   └── 02_exploratory_analysis.ipynb
│
├── src/
│   └── data_cleaning.txt
│
├── powerbi/
│   └── sales_dashboard.pbix
│
└── reports/
    └── figures/
```

## Directory structure explanation

| Directory | Purpose |
|---|---|
| `docs/` | Project documentation, data definitions, and business findings. |
| `data/raw/` | Original, unmodified datasets. |
| `data/processed/` | Cleaned and transformed datasets. |
| `sql/` | SQL scripts for data validation, exploration, KPI analysis, and advanced analytics. |
| `notebooks/` | Jupyter notebooks for exploratory data analysis. |
| `src/` | Reusable Python scripts for data cleaning and transformation. |
| `powerbi/` | Power BI dashboard files. |
| `reports/figures/` | Exported charts and dashboard screenshots. |

| File | Description |
|---|---|
| `project_brief.md` | Business problem, objectives, stakeholders, and analytical questions. |
| `data_dictionary.md` | Dataset schemas, column definitions, and data types. |
| `findings.md` | Analytical findings and business recommendations. |
| `data_cleaning.py` | Reusable Python ETL and data-cleaning pipeline. |
| `requirements.txt` | Python dependencies required to run the project. |

# Limitations of this repository

GitHub is my version-control and documentation home, not necessarily the place where my entire project runs. A Power BI .pbix file may require Power BI Desktop to inspect, and database setup may require separate instructions.
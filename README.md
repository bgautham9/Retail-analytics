# Retail Analytics End-to-End Project (Power BI)

## Project Overview
This project simulates a real-world retail analytics workflow using messy business data and Power BI.

The focus of this project is not just dashboard creation, but understanding how raw business data is cleaned, validated, standardized, and prepared before analysis.

The dataset intentionally contains:
- inconsistent category values
- mixed casing
- hidden formatting issues
- invalid business values
- duplicate-like records
- inconsistent region naming

This project is being built step-by-step to simulate actual analyst workflow in enterprise environments.

---

# Project Goals

- Perform realistic data cleaning using Power Query
- Handle business data inconsistencies
- Validate numerical and categorical fields
- Build repeatable transformation workflows
- Create an end-to-end analytics project
- Document analyst decisions and challenges
- Build professional Power BI portfolio project

---

# Tools Used

- Power BI Desktop
- Power Query
- GitHub
- CSV Files

---

# Dataset Structure

## Raw Monthly Files
- orders_jan.csv
- orders_feb.csv
- orders_mar.csv

## Master Dataset
- full_company_dataset.csv

---

# Current Progress

## Phase 1 — Data Audit
Completed:
- reviewed raw datasets
- identified inconsistencies
- documented data quality issues
- created project folder structure
- uploaded raw files to GitHub

---

## Phase 2 — Data Cleaning & Standardization
Completed using Power Query:

### Data Consolidation
- appended monthly CSV files into one combined dataset
- validated schema consistency across files

### Data Profiling
Enabled:
- Column Quality
- Column Distribution
- Column Profile

Used profiling to identify:
- invalid values
- hidden inconsistencies
- duplicate categories
- business anomalies

---

# Cleaning Tasks Completed

## Region Standardization
Fixed inconsistencies like:
- East
- east
- EAST
- Est

Final standardized regions:
- East
- West
- South
- Central

---

## Category Standardization
Fixed inconsistent values like:
- tech
- Tech
- Officesupply
- Furnitureiture

Final standardized categories:
- Furniture
- Office Supplies
- Technology

---

## Segment Standardization
Standardized:
- Consumer
- Corporate
- Home Office

Handled hidden blank values affecting distinct counts.

---

## Data Cleaning Transformations Used

Applied:
- Trim
- Clean
- Capitalize Each Word
- Replace Values
- Filter Rows

---

## Discount Validation

Identified invalid business values:
- negative discounts
- discounts above 100%

Applied business rule filtering:
- kept only discount values between 0 and 1

---

# Real-World Challenges Faced

## Hidden Formatting Issues
Some values looked identical visually but contained:
- trailing spaces
- hidden characters
- formatting inconsistencies

Resolved using:
- Trim
- Clean transformations

---

## Transformation Side Effects
While replacing category values:
Furniture → Furnitureiture

This highlighted the importance of validating transformations carefully after every replacement operation.

---

## Profiling Limitations
Power Query profiling initially analyzed only top 1000 rows, causing misleading distinct counts.

Resolved by switching profiling to:
- entire dataset analysis

---
Phase 3 — Transaction Validation & Date Handling

sales validation
quantity filtering
negative profit analysis
date parsing issue
business-rule validation

# Key Learning

One of the biggest learnings from this project:

Good dashboards depend on trusted and standardized data.

Most analytics effort happens before visualization.

---

# Next Steps

Upcoming phases:

- Data modeling
- DAX measures
- KPI dashboards
- Business insights generation

---

# Repository Structure

```text
Retail-Analytics
│
├── raw_data
│   ├── orders_jan.csv
│   ├── orders_feb.csv
│   ├── orders_mar.csv
│
├── processed_data
│
├── screenshots
│
├── business_notes
│
├── powerbi
│
└── README.md

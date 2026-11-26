# Raw Data Layer

## Purpose

This directory serves as the raw source data repository for CineScope AI.

Datasets stored within this directory represent original source inputs prior to data cleaning, standardization, transformation, enrichment, or feature engineering.

## Data Governance Principles

- Preserve original source data without modification.
- Maintain source data version history through Git version control.
- Document dataset provenance, acquisition methodology, and known limitations.
- Maintain traceability between source datasets and downstream data processing activities.
- Perform cleaning and transformation operations outside the raw data layer.
- Require appropriate verification and qualification before approving datasets for analytical or predictive use.
- Confirm applicable licensing and redistribution permissions before publishing source datasets.

## Dataset Inventory

| Dataset | Description | Qualification Status |
|---|---|---|
| `box_office_2026.csv` | Original 2026 Movie Box Office Report dataset | Not Qualified |

## Current Data Quality Disposition

The initial 2026 box office dataset has undergone a preliminary data quality audit within `notebooks/01_data_audit.ipynb`.

The audit identified outstanding data quality, source verification, and dataset coverage limitations requiring remediation.

The dataset is currently restricted to controlled development, data quality assessment, remediation, and qualification activities.

## Usage Restrictions

The presence of a dataset within this directory does not constitute:

- Source verification
- Data quality approval
- Analytical approval
- Predictive modeling approval
- Production deployment authorization

All downstream usage remains subject to documented qualification requirements and governance controls.

## Data Integrity

Raw source datasets must not be overwritten with cleaned or transformed values.

Processed datasets will be maintained separately within the `data/processed/` directory.

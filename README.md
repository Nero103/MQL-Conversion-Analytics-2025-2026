# MQL Conversion Tracker (Synthetic Demo Project)
## Overview

This repository contains a synthetic B2B funnel analytics project built using **Tableau** and **Tableau Prep**. The purpose of this project is to demonstrate data preparation techniques and funnel visualization using mock datasets.

All data in this repository is artificially generated for portfolio demonstration and does not represent any real organization.

The project models how qualified leads can progress through multiple funnel stages and ultimately convert into closed opportunities.

## Data Pipeline Process
### 1. Combining Lead Sources

Multiple synthetic datasets representing inbound leads and contacts were cleaned and merged to form a unified lead dataset. This step demonstrates how Tableau Prep can be used to standardize fields and combine sources for funnel analysis.

### 2. Funnel Stage Modeling

The unified dataset was segmented into generic funnel stages:

**Accepted Leads**

**Qualified Leads**

**Qualified Opportunities**

**Closed Opportunities**

Each stage was processed independently before being recombined into a single funnel dataset.

### 3. Funnel Consolidation

All funnel stages were unioned into one consolidated dataset to support time-based conversion analysis and visualization.

### 4. Workflow Overview Breakdown

This project demonstrates how to build a multi-stage funnel analytics pipeline using Tableau Prep and Tableau with synthetic data.

 The workflow follows a modular ETL-style design:

#### 1. Source Preparation

Multiple mock datasets representing inbound prospects were ingested into Tableau Prep. Each source was independently cleaned and standardized to ensure consistent field formats (dates, IDs, and stage indicators).

Basic filtering was applied to remove incomplete records and enforce valid funnel entry criteria.

#### 2. Lead Consolidation

Separate prospect sources were combined into a unified dataset using union operations. This step simulates how multiple acquisition channels can be merged to create a single lead population for analysis.

This unified dataset serves as the starting point for all downstream funnel calculations.

#### 3. Funnel Stage Segmentation

The consolidated dataset was split into individual funnel stages based on synthetic status indicators:

- Accepted Leads

- Qualified Leads

- Qualified Opportunities

- Closed Opportunities

Each stage was processed independently to:

- **Normalize timestamps**

- **Apply stage-specific filters**

- **Prepare metrics for aggregation**

This modular approach allows each funnel step to be validated separately before recombining.

#### 4. Aggregation and Metric Calculation

For each funnel stage, aggregated metrics were calculated, including:

- Record counts by month

- Stage-to-stage conversion rates

- Progression volume across the funnel

- These aggregated outputs were then recombined into a single unified funnel table.

#### 5. Final Funnel Assembly

All stage-level datasets were unioned into a final analytical table that represents the complete synthetic funnel lifecycle.

This dataset was structured to support:

- Month-over-month trend analysis

- Funnel conversion visualization

- Performance benchmarking

#### 6. Visualization Layer

The final dataset was published to Tableau and used to create an interactive dashboard showing:

- Funnel volume by stage

- Conversion percentages between stages

- Time-based trends

- The dashboard provides a clear view of how leads progress through the pipeline and where drop-off occurs.

- Design Principles

**The workflow emphasizes:**

- Modular Prep steps for clarity and debugging

- Explicit stage isolation for accurate funnel measurement

- Aggregation prior to visualization for performance

- Separation of preparation and presentation layers

- This approach mirrors common analytics engineering patterns used in real-world BI environments.

## Final Output

The final dataset was used to build a Tableau dashboard illustrating lead progression across funnel stages and highlighting conversion trends over time.

Technologies Used

**Tableau Prep** – data cleaning, unions, and transformations

**Tableau** – dashboard creation and visualization

**SQL** – exploratory data preparation

## Confidentiality Notice

All datasets and workflows in this repository are synthetic and created solely for portfolio demonstration purposes. No proprietary, confidential, or employer-derived information is included. Metrics and values do not represent any real organization.

## Conclusion

This project demonstrates practical techniques for building funnel analytics using Tableau Prep and Tableau, including data consolidation, stage modeling, and visualization of conversion performance.

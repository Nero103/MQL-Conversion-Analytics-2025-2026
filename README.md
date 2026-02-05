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

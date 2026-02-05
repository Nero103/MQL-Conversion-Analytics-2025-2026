# MQL Conversion Tracker
## Overview

This repository contains a MQL (Marketing Qualified Lead) Conversion Tracker, built using Tableau and Tableau Prep. The goal of this project is to track the movement of leads through the sales funnel from **Sales Accepted Lead (SAL)** to **Sales Qualified Lead (SQL)** **Sales Qualified Opportunity (SQO)** to **Won Opportunities**.

The project utilizes Tableau Prep to combine and clean multiple datasets, filter leads and contacts, and merge them into a single dataset that enables detailed sales funnel analysis and reporting. The final dataset was used to build a Tableau dashboard that visualizes the MQL conversion process.

## Data Pipeline Process
### 1. Union of Lead MQLs and Contact MQLs

The first step in the data preparation process was to union the **Lead MQLs** and **Contact MQLs** into a complete set of data. This step was necessary to ensure that both leads and contacts were captured in the sales funnel, allowing for a complete count of MQLs.

Filtered Leads and Contacts: Both leads and contacts were filtered based on business requirements to ensure that only relevant records were included.

Union Operation: The filtered leads and contacts datasets were unioned to form a combined set of MQLs.

### 2. Account Data Joins

To enhance the dataset and include the necessary account-level information, joins were used to merge the Account Table with the unified MQLs (Leads + Contacts) dataset. This step allowed for the inclusion of critical account-level attributes, including the last dates for each funnel stage.

Merged Accounts with Clean Steps: Joined account data to the cleaned steps dataset to ensure that the appropriate last dates for each funnel stage were correctly included.

Filtered by Stages: The data was then filtered based on their respective stage data tables to ensure that each MQL could be tracked through the funnel stages (Lead to Accepted to Qualified to Opportunity).

### 3. Funnel Data Preparation

After filtering and joining the data, the next step was to isolate the four funnel categories into their own datasets. These categories were:

**Sales Accepted Leads (SAL)**

**Sales Qualified Leads (SQL)**

**Sales Qualified Opportunities (SQO)**

**Won Opportunities**

Union of Funnel Datasets: These isolated datasets were unioned into a single dataset, which was then unioned again with the Lead + Contact MQLs dataset. This final union ensured that we had a comprehensive funnel dataset for analysis.

### 4. Final Output

The final output was a unified funnel dataset containing all the necessary stages for the sales funnel analysis. This dataset was used to create the Tableau view, which visualized the MQL conversion process, showing the movement of MQLs from creation to won opportunities.

## Technologies Used

**Tableau Prep:** For data cleaning, filtering, union, and joins to create a unified dataset.

**Tableau:** For creating the final dashboard and visualizing the MQL conversion funnel.

**SQL:** For querying and manipulating the data prior to using Tableau Prep.

## Files in this Repository

Tableau Prep Flow File: Contains the step-by-step flow used to clean, union, and join datasets.

Tableau Workbook: Contains the final view/dashboard displaying the MQL funnel and conversion rates.

## Conclusion

This project demonstrates the power of Tableau Prep for data preparation and sales funnel analysis. By unioning and cleaning data from different sources (leads, contacts, accounts), we created a consolidated dataset that allowed us to track and analyze MQLs as they progress through the sales pipeline. The final visualization in Tableau provides clear insights into the efficiency of each stage in the funnel, driving data-informed decisions for optimizing lead qualification and sales performance.

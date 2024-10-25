# Project Overview

This project aims to analyze missed appointments, also known as Did Not Attends (DNAs), within the National Health Service (NHS) network. By focusing on key components of appointment scheduling and workforce utilization, the analysis will help the NHS improve healthcare accessibility, efficiency, and resource utilization. The results of this analysis will inform decision-making regarding budget allocation, capacity expansion, and the optimal use of existing resources across the NHS.

## Key Objectives

1. **Evaluate Staff Capacity & DNAs**  
   Assess whether there has been sufficient staff and appointment capacity, and how these factors relate to the rate of missed appointments (DNAs).

2. **Assess Resource Utilization Across the Network**  
   Determine the level of resource utilization in healthcare facilities across the NHS network, identifying gaps or inefficiencies.

## Data Sources

The analysis integrates multiple datasets at different granularities. The primary datasets used include:

### Primary Datasets:
- **actual_duration.csv (AD)**
- **appointment_regional.csv (AR)**
- **national_categories.csv (NC)**

### Supplementary Datasets:
- **GP_STATS**:  
  Provides Full-Time Equivalent (FTE) data, focusing on NHS general practice workforce utilization. The dataset is extracted from the NHS General and Personal Medical Services statistics publication. It contains data aggregated by region and Sub-ICB location from December 2021 to June 2022. Please note that data collection methodologies changed after December 2021.

  For more details on GP_STATS, refer to the full bulletin publication:  
  [NHS General and Personal Medical Services](https://digital.nhs.uk/data-and-information/publications/statistical/general-and-personal-medical-services)

- **Geographic Data**:  
  Geographic data has been imported from the UK GeoPortal to provide additional regional and Sub-ICB information. These geographic codes (`ICB_ons_code`, `sub_ICB_location`) are essential for merging and analyzing datasets across different geographic levels.

  Learn more about the geographic data:  
  [GeoPortal Documentation](https://geoportal.statistics.gov.uk/documents/46b634b42ceb45cbbfbe9c960fb77ec9/about)

### Social Media Dataset:
- **Tweet.csv**:  
  Scraped data from Twitter (now X) used for sentiment analysis related to NHS appointments and healthcare access.

**Metadata**: See `metadata_nhs.md` for detailed information on each dataset.

## Tools Used 
Python used for data ingestion, wrangling and analysis. 
GitHub for version control and project management

## Analysis
Since we were interested in understanding trends and patterns in the newtwork, we focused on analysis of locations, trends over time, appointemnt types and service setting provider.
Analysis has been divided into univariate and bivariate statistics to understand the trend in the variation of appointments and their attributes over time and across networks. 
The analysis covers the period from June 2020 to June 2021, to minimize anomalies caused by the COVID-19 pandemic.

### Diagnostic Analysis and Insights

- **Utilization Trends**:  
  Analyzes the utilization of NHS services across different regions and appointment types.
  
- **Missed Appointments**:  
  Investigates missed appointments (DNAs) and their potential causes, looking into patterns that may correlate with staff shortages or other capacity issues.

- **Sentiment Analysis**:  
  Uses external data sources like Twitter (X) for sentiment analysis on public perception of NHS services. Sentiment scores were calculated using the TextBlob library, which provides insights into the public's mood regarding NHS appointments and access to healthcare services.


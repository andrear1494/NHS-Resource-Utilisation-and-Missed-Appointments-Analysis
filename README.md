# Project Overview

This project aims to analyze missed appointments, also known as Did Not Attends (DNAs), within the National Health Service (NHS) network. By focusing on key components of appointment scheduling and workforce utilization, the analysis will help the NHS improve healthcare accessibility, efficiency, and resource utilization. The results of this analysis will inform decision-making about budget allocation, expansion of capacity, and the optimal use of existing resources across the NHS.

### Key Objectives:
1. **Evaluate Staff Capacity & DNAs**  
   Assess whether there has been sufficient staff and appointment capacity, and how these factors relate to the rate of missed appointments (DNAs).
   
2. **Assess Resource Utilization Across the Network**  
   Determine the level of resource utilization in healthcare facilities across the NHS network, identifying gaps or inefficiencies.

## Data Sources

The analysis integrates multiple datasets at different granularities. The primary datasets used include:

### Primary Datasets:
1. **actual_duration.csv (AD)**     
2. **appointment_regional.csv (AR)**     
3. **national_categories.csv (NC)**  

### Supplementary Datasets:
1. **GP_STATS**  
   Provides Full-Time Equivalent (FTE) data, focusing on NHS general practice workforce utilization. The dataset is extracted from the NHS General and Personal Medical Services statistics publication. It contains data aggregated by region and Sub ICB location from December 2021 to June 2022. Please note that data collection methodologies changed after December 2021.

   For more details on GP_STATS, refer to the full bulletin publication:  
   [NHS General and Personal Medical Services](https://digital.nhs.uk/data-and-information/publications/statistical/general-and-personal-medical-services)

2. **Geographic Data**  
   Geographic data has been imported from the UK GeoPortal to provide additional regional and sub-ICB information. These geographic codes (ICB_ons_code, sub_ICB_location) are essential for merging and analyzing datasets across different geographic levels.

   Learn more about the geographic data:  
   [GeoPortal Documentation](https://geoportal.statistics.gov.uk/documents/46b634b42ceb45cbbfbe9c960fb77ec9/about)

### Social Media Dataset:
1. **Tweet.csv**  
   Scraped data from Twitter (now X) used for sentiment analysis related to NHS appointments and healthcare access.
   
### Metadata: See metadata_nhs

## Analysis
Since we were interested in understanding trends and patterns in the newtwork, we  focused on analysis of locations, trends over time, appointemnt types and service setting provider.  
Analysis has been divided into univariate and bivariate statistics to understand the trend in the variation of appointments and their attributes over time and across networks.  We looked at the period June 2020-June 2021 to minimise anomalies caused by Covid-19.

**Diagnostic Analysis and Insights includes**: 
- **Utilization Trends**: Analysis related to the utilization of services. 
- **Missed Appointments**: Analysis related to missed appointments and potential causes.
- **Sentiment Analysis** involving external data sources like Twitter (X) using TextBlob library. 



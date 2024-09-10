**This is my first work assignment on Python!**

**Business context:**
The National Health Service (NHS) aims to address missed appointments, known as Did Not Attends (DNAs), to enhance healthcare accessibility, efficiency, and resource utilisation.
This specific analysis will inform decision-making regarding the utilisation trends of each component of the network. In particular, it will focus on two overarching objects: 
1.	Evaluate whether there has been adequate staff and capacity and if this related to DNAs 
2.	Determine the resource utilisation across the network 
This report will inform decision-making regarding budget allotment, whether to expand capacity or improve utilisation of existing resources within the NHS.

**Data:**
The analysis encompasses the use of appointment datasets at different granularities : actual_duration.csv, appointment_regional.csv, national_categories.csv and 3 primary appointment datasets (AD, NC, NR )  and integrates findings with additional FTE data (GP_STATS)  to assess the primary care workforce utilisation. 
GP_STATS is an extract from the NHS GENERAL PRACTICE STATS. Here, you can see the full bulletin publication:   
https://digital.nhs.uk/data-and-information/publications/statistical/general-and-personal-medical-services
Note that the data collection methodologies have changed since December 2021. The series are now published monthly and aggregated by Regions and Sub ICB Location instead of quarterly. This version is an extract of the data available with these granularities from December 2021 to June 2022.

Geographic data have also been imported to extract regional and sub-ICB level information, providing keys to merge all datasets using ICB_ons_code or sub_ICB_location.
https://geoportal.statistics.gov.uk/documents/46b634b42ceb45cbbfbe9c960fb77ec9/about

**Analysis**: 
Since we were interested in understanding trends and patterns in the newtwork, we  focused on analysis of locations, trends over time, appointemnt types and service setting provider.  
Analysis has been divided into univariate and bivariate statistics to understand the trend in the variation of appointments and their attributes over time and across networks.  We looked at the period June 2020-June 2021 to minimise anomalies caused by Covid-19.

**Diagnostic Analysis and Insights includes**: 
**Utilization Trends**: Analysis related to the utilization of services. 
**Missed Appointments**: Analysis related to missed appointments and potential causes.
**Sentiment Analysis** involving external data sources like Twitter (X) using TextBlob library. 



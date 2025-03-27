# 🏥 COVID-19 Data Engineering Project

## 📌 Project Objective
The goal of this project was to build a scalable data pipeline to analyze COVID-19 trends, mortality rates, and public health impacts. By ingesting and processing data from ECDC and Eurostat, I created a system to track infection rates, hospitalizations, and demographic impacts using Azure Data Factory and Databricks.

## 🏗️ Architecture Diagram
<img width="647" alt="image" src="https://github.com/user-attachments/assets/fab3f22f-7ec0-4a46-9724-e0ed4129bc32" />

## 🔍 Key Questions Explored
- Which age groups were most vulnerable to severe outcomes?
- How did hospitalization rates correlate with case numbers?
- What was the impact of testing strategies on case detection?
- How did mortality rates vary by country and demographic?
- What were the trends in ICU occupancy during peak waves?

## 🚀 Tech Stack
**Cloud**: Microsoft Azure  
**Data Processing**: Databricks (PySpark, Spark SQL)  
**Storage**: Azure Data Lake Storage Gen2  
**Data Ingestion**: Azure Data Factory (HTTP, Blob Storage connectors)  
**Data Transformation**: PySpark, Delta Lake  
**Orchestration**: ADF Pipelines with Schedule/Event Triggers  
**Visualization**: Power BI  
**DevOps**: Azure DevOps (CI/CD pipelines)

## 📊 Insights & Findings

### 🦠 1. Infection Trends
- Countries with older populations showed significantly higher mortality rates
- Clear waves of infection correlated with seasonal changes and policy changes
- Weekly reporting transitions (Page 75) required pipeline adjustments

### 🏥 2. Healthcare System Impact
- ICU occupancy typically peaked 1-2 weeks after case surges
- Hospitalization rates showed strong correlation with cases in older demographics
- Mortality rates improved significantly post-vaccination rollout

### 🧪 3. Testing Analysis
- Countries with higher testing rates detected cases earlier
- Positivity rates above 10% consistently signaled uncontrolled spread
- Testing data became more reliable after standardization in 2021

## 🏗️ Project Workflow

### Data Ingestion
- Collected COVID-19 data from ECDC via HTTP connector (Page 76-80)
- Ingested population data from Eurostat via Azure Blob Storage (Page 50-61)
- Implemented robust error handling for source data changes (Page 75)

### Data Processing
- Used Databricks pyspark 
- Used DataFlow for minor Changes.

### Data Orchestration
- Used ADF pipelines with:
  - Schedule triggers for weekly updates
  - Event triggers for ad-hoc data loads
  - Dependency chaining between activities

### Data Visualization
- Built Power BI dashboards showing:
  - Case fatality rates by age group
  - Hospitalization trends over time
  - Geographic distribution of cases

## 📊 Power BI Dashboards (Key Metrics)
- **Infection Trends**: 14-day case rates by country
- **Healthcare Impact**: Hospital/ICU occupancy vs. capacity
- **Demographic Analysis**: Age-stratified mortality rates
- **Testing Efficacy**: Positivity rates vs. testing volume

## 🎯 Conclusion
This project created a robust framework for analyzing COVID-19 data, revealing critical insights about transmission patterns, healthcare system impacts, and demographic vulnerabilities. The pipeline is designed to handle evolving data formats and reporting schedules.

## 🤝 Future Enhancements
- **Real-time Alerting**: Integrate streaming data for early warning
- **Predictive Modeling**: Forecast regional outbreaks
- **Vaccination Analysis**: Incorporate immunization data
- **Policy Impact**: Measure effectiveness of interventions

## 📞 Contact
For questions or collaborations:
[LinkedIn Profile](https://www.linkedin.com/in/srinivas-gupta-veerabomma/)

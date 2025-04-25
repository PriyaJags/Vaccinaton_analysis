# Vaccination Data Analysis and Visualization

## Project overview
Analyze global vaccination data to understand trends in vaccination coverage, disease incidence, and effectiveness. Data is cleaned, and stored in a SQL database. Power BI is used to connect to the SQL database and create interactive dashboards that provide insights on vaccination strategies,provide actionable insights for public health strategy, disease prevention, and resource allocation.

## Skills Gained
- Python for data cleaning and exploration  
- SQL for structured data storage and querying  
- Power BI for building interactive dashboards  
- Exploratory Data Analysis (EDA)  
- Domain knowledge in public health and epidemiology

## Domain
**Public Health and Epidemiology**

## Problem Statement

Analyze global vaccination data to:
- Understand trends in vaccination coverage and disease incidence
- Evaluate vaccine effectiveness over time
- Identify gaps in coverage and areas needing public health intervention

## Business Use Cases

### 1. Public Health Strategy
- Evaluate vaccination effectiveness across regions and demographics  
- Identify low-coverage areas for targeted intervention

### 2. Disease Prevention
- Spot high disease incidence despite vaccinations  
- Support booster policies and new vaccine rollouts

### 3. Resource Allocation
- Distribute vaccines to under-vaccinated regions  
- Forecast vaccine demand and optimize supply chains

### 4. Global Health Policy
- Support evidence-based vaccination policies  
- Help organizations meet global immunization goals

##  Approach

###  Data Cleaning (Python)
- Handle missing values
- Normalize units and fields (coverage %, cases, etc.)
- Ensure consistent date formats

###  SQL Database Setup
- Create and normalize relational tables: vaccines, diseases, coverage, incidencerate, reportedcases, vaccineschedule, vaccineintro, whoregions, years etc.
- Add primary/foreign keys for referential integrity

###  Power BI Integration
- Connect Power BI to SQL database
- Build interactive dashboards with filters and slicers

###  Visualizations
- Line and bar charts for yearly trends  
- Scatter plots showing coverage vs. incidence  
- KPI cards for progress tracking
- slicers for country , years, disease and showing corresponding trends

##  Exploratory Data Analysis (EDA)

Performed statistical summaries and visualizations to:
- Track vaccine trends
- Understand disease dynamics
- Identify regional or demographic disparities

##  Key Questions Answered
- Determine how vaccination rates vary over the years.
- Determine disease incidence rates over the years.
- How do vaccination rates correlate with a decrease in disease incidence?
- What is the drop-off rate between 1st dose and subsequent doses?.
- Are vaccination rates different between genders?
- What is the urban vs. rural vaccination rate difference?
- Has the rate of booster dose uptake increased over time?
- Is there a seasonal pattern in vaccination uptake?
- How do vaccination rates correlate with a decrease in disease incidence?
- Which regions have high disease incidence despite high vaccination rates?
- Is there a correlation between vaccine introduction and a decrease in disease cases?
- Which diseases have shown the most significant reduction in cases due to vaccination?
- What percentage of the target population has been covered by each vaccine?
- Are there significant disparities in vaccine introduction timelines across WHO regions?
- How does vaccine coverage correlate with disease reduction for specific antigens?
- Are certain diseases more prevalent in specific geographic areas?
- estimate vaccine demand for a specific disease over year
- track global progress toward achieving a target of 95% vaccination coverage

##  Technologies Used

- **Python** – Data cleaning & EDA  
- **MySQL** – Relational database  
- **Power BI** – Dashboards & Visual Analytics  
- **GitHub** – Version control and documentation

##  Datasets Overview

| Table | Variables |
|-------|-------------|
| **Coverage** |Group, Code, Name, Year, Antigen, Antigen_description, Coverage_category, Coverage_category description, Target number, doses, Coverage |
| **Incidence Rate** | Group, Code, , Name, Year, Disease, Disease description, Denominator, Incidence rate  : Classification of the data; here, it represents countries.|
| **Reported Cases** |Group, Code, Name, Year, Disease, Disease description, Cases|
| **Vaccine Introduction** | ISO_3_Code, Country Name,,  Who Region, Year, Description, Intro  : Unique 3-letter ISO country code.|
| **Vaccine Schedule** | ISO_3_Code, Country Name, Who Region, Year, Vaccine code, Vaccine description, Schedule rounds, Target pop, Target pop description, Geoarea, Age administered, Source comment.|


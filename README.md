# Power Bi- Energy - Dashboard
Power BI dashboard analyzing renewable energy production in France to support strategic network planning and investment decisions.

# Project Overview
This project consists of an interactive Power BI dashboard designed to monitor and analyze the evolution of renewable energy production connected to the French electricity distribution network, with a focus on data provided for Enedis.

The dashboard supports strategic decision-making related to energy transition, network planning, and investment prioritization.

# Business Context
Enerdata, a company specialized in energy data analytics, was commissioned by Enedis to conduct an in-depth analysis of the evolution of renewable energy production assets connected to the distribution network in France.

The objective was to provide Enedis’ Network Studies & Forecasting Department with a dynamic and interactive reporting tool to:

  - Monitor the growth of renewable energy installations,

  - Anticipate changes in the local energy mix,

  - Identify high-potential geographic areas,

Support strategic investment and infrastructure planning decisions,
in line with energy transition and climate objectives.

# Data Sources
The analysis is based on multiple reliable and institutional data sources:

🔹 Enedis – Renewable Energy Production Assets

Summary dataset of renewable energy production assets connected to the French distribution network (2020–2025)

Unit: Megawatt (MW), representing installed capacity (maximum production capacity of an installation)

🔹 Météo-France – Temperature Data (2020–2025)

Average temperature data (°C)

Used to enrich the analysis and provide environmental context

🔹 Energy Type Reference Dataset

Classification of renewable energy types included in the study:

Photovoltaic 

Wind 

Hydropower 

Bioenergy 

Cogeneration 

Non-hydraulic storage 

Other renewable sources 

🔹 Solar Irradiance Data

Sunshine duration dataset for 2024, by French department

Measures the number of hours during which direct solar radiation exceeds a defined threshold

Used to estimate potential photovoltaic productivity

_All datasets used in this project are public, educational, or anonymized, and are intended for analytical and demonstration purposes only_

# Data Modeling & Transformations

🔹 Data Preparation

Data cleaning and transformation were performed using Power Query to ensure data consistency, reliability, and analytical usability.

Key steps included:

Standardization of column names and data types

Handling missing and inconsistent values

Harmonization of geographic identifiers (French departments)

Creation of a clean and analysis-ready dataset

🔹 Data Model Design

The Power BI data model follows a star schema design to optimize performance and analytical clarity.

- Fact table

Renewable energy production capacity (MW)

- Dimension tables

Date

Energy type

Geographic area (department / region)

Weather and solar context

This structure enables efficient filtering, drill-down analysis, and time intelligence calculations

🔹 Enrichment & Business Logic

Integration of weather and solar irradiance data to contextualize production capacity

Mapping of renewable energy types using standardized classification codes

Creation of calculated fields and measures to support KPI analysis

🔹 Performance Optimization

Reduction of data granularity when necessary

Removal of unused columns

Optimized relationships to improve report responsiveness

# Key Insights & Business Value

This dashboard provides actionable insights to support strategic planning and investment decisions related to renewable energy integration into the French electricity distribution network.

🔹 Growth of Renewable Energy Capacity

A steady increase in installed renewable energy capacity is observed between 2020 and 2025, reflecting the acceleration of France’s energy transition

Wind and photovoltaic energy emerge as the primary drivers of this growth

🔹 Geographic Disparities

Significant regional disparities exist in terms of installed capacity and growth rates

Certain departments show high development potential, indicating priority areas for future infrastructure investments

🔹 Energy Mix Evolution

The renewable energy mix is progressively diversifying, reducing dependency on a single energy source

This diversification contributes to greater network resilience and risk mitigation

🔹 Environmental Context & Productivity

The integration of temperature and solar irradiance data highlights correlations between environmental conditions and renewable energy deployment

Departments with higher sunshine duration demonstrate stronger photovoltaic productivity potential

🔹 Strategic Value for Decision-Makers

The dashboard enables stakeholders to:

 - Anticipate future network constraints

 - Optimize grid reinforcement planning

 - Prioritize investments based on regional potential

# Key Analytical Measures

 - Total Installed Renewable Capacity (MW)
   
Represents the total installed renewable energy capacity connected to the distribution network, aggregated across all energy types, regions, and selected periods

Used to monitor global growth trends and assess infrastructure scale requirements

- Share of Installations with Storage

Calculates the proportion of renewable energy installations equipped with storage solutions

Helps evaluate grid flexibility and storage adoption in support of intermittent energy sources

- Photovoltaic Yield Indicator

An estimated indicator that combines installed photovoltaic capacity with regional sunshine levels to evaluate solar energy potential

Helps identify regions with higher photovoltaic potential and supports investment decisions

_Exact calculation logic is intentionally simplified for portfolio purposes._

# Dashboard Pages

__Renewable Energy Overview__

Global evolution of renewable installations and installed capacity, breakdown by energy type and year

Allows decision-makers to quickly assess overall growth trends and structural changes in the renewable energy landscape

__Regional & Departmental Analysis__

Analyze renewable energy deployment at regional and departmental levels

Identifies high-potential geographic areas for future investments

__Climate & Photovoltaic Potential__

Assess the relationship between environmental conditions and photovoltaic energy potential

Supports photovoltaic site selection and long-term planning

__Storage & Grid Flexibility__

Provides insights into grid flexibility and readiness for renewable integration

# Limitations

Analysis is based on installed capacity (MW) rather than actual energy production (MWh)

Theoretical photovoltaic yield is an indicative metric, not a real production forecast

Data updates are periodic and not real-time















_This project is shared for portfolio and demonstration purposes only. Any reuse without attribution is prohibited._




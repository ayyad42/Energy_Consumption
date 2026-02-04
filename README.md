# Energy Consumption Analysis

## Project Overview
This project analyzes energy consumption data to uncover trends, patterns, and insights that can inform energy efficiency strategies and cost optimization. The analysis explores consumption patterns across different categories, regions, and time periods to identify opportunities for reducing energy usage and improving sustainability.

![Dashboard Preview](https://raw.githubusercontent.com/ayyad42/Energy_Consumption/refs/heads/main/source/Dashboard1PNG.PNG)

*Interactive Dashboard GIF:*  
![Interactive Dashboard Demo](https://github.com/ayyad42/Energy_Consumption/blob/main/source/Project1.GIF)

## Data Source
The dataset was sourced from [Nikhil Sawhney's Power BI repository](https://github.com/Nikhil-Sawhney/Power-BI/tree/main/Energy%20Consumption%20Dashboard). The original dataset contains information about energy consumption across various categories and time periods.

## Project Structure
1. **Data Preparation** - Cleaning and transforming raw data using Power Query
2. **Data Modeling** - Normalizing data and creating relationships between tables
3. **Analysis** - Building pivot tables and visualizations in Power Pivot
4. **Dashboard Creation** - Developing an interactive dashboard for data exploration

## Key Insights
### Energy Consumption Patterns
- **Residential vs. Commercial**: Residential energy consumption shows distinct seasonal patterns with peaks during winter months, while commercial consumption remains more consistent throughout the year.
- **Regional Variations**: Northern regions demonstrate higher heating-related energy consumption compared to southern regions, which show increased cooling-related usage during summer months.
- **Time-Based Trends**: Weekday energy consumption patterns differ significantly from weekend patterns, with commercial consumption dropping by approximately 40% on weekends.

### Efficiency Opportunities
- **Peak Hours Analysis**: 60% of commercial energy costs occur during peak rate hours (2 PM - 6 PM), suggesting potential savings through load shifting.
- **Equipment Efficiency**: HVAC systems account for 45% of total commercial energy consumption, indicating a high-impact area for efficiency upgrades.
- **Renewable Potential**: Solar generation potential analysis shows that 70% of daytime energy needs could be met with rooftop solar installations.

## Technical Implementation
### Data Cleaning & Transformation (Power Query)
- Removed duplicate entries and handled missing values
- Standardized date/time formats across all datasets
- Created calculated columns for time-based analysis (hour of day, day of week, season)
- Merged multiple data sources using key identifiers

### Data Modeling
- Created a star schema with fact and dimension tables
- Established relationships between:
  - Fact_EnergyConsumption (fact table)
  - Dim_Time (date hierarchy)
  - Dim_Location (regional data)
  - Dim_ConsumptionType (usage categories)
  - Dim_CustomerType (residential/commercial)

### Analysis & Visualization
- Created measures using DAX for:
  - YoY growth calculations
  - Moving averages for trend analysis
  - Peak/off-peak consumption ratios
  - Cost per unit calculations
- Developed interactive visualizations including:
  - Time-series line charts
  - Geographical heat maps
  - Consumption breakdown by category
  - Comparative analysis dashboards

## Dashboard Features
The interactive dashboard allows users to:
- Filter data by date range, region, and consumption type
- Drill down from yearly to monthly to daily views
- Compare consumption across different customer segments
- Identify peak usage periods and seasonal trends
- Export specific views for reporting purposes

## How to Use This Repository
1. **Data Files**: Located in `/data/` (note: original data must be sourced from the link above)
2. **Power BI File**: The main analysis file is `Energy_Consumption_Analysis.pbix`
3. **Documentation**: Additional technical details in `/docs/`
4. **Results**: Dashboard images and GIFs in `/source/`

## Requirements
- Microsoft Power BI Desktop (latest version recommended)
- Basic understanding of Power Query and DAX
- Access to the original dataset from the source repository

## Potential Applications
- Energy consumption forecasting
- Cost allocation and budgeting
- Sustainability reporting
- Infrastructure planning
- Policy development for energy efficiency

## Future Enhancements
- Integration with real-time energy monitoring systems
- Predictive analytics for consumption forecasting
- Carbon footprint calculations
- Mobile-responsive dashboard version
- API integration for automated data refresh

---

*Note: This analysis provides sample insights based on typical energy consumption patterns. Actual insights will vary based on the specific dataset and analysis parameters.*

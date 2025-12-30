# Agri-Data-Explorer
Project Overview : This project performs an Exploratory Data Analysis on Indian agricultural datasets to understand the relationship between various types of crops its area, production and yield. The goal is to identify trends across states, detect outliers, and understand the efficiency of land usage.
1. Dataset Description:
   Source: ICRISAT-District_Level_Data.csv
   Time Period: 1966- 2017
   Features:
        dist_code, year, state_code, state_name, dist_name,
       rice_area_1000_ha,rice_production_1000_tons,
       rice_yield_kg_per_ha,wheat_area_1000_ha,
       wheat_production_1000_tons,wheat_yield_kg_per_ha,
       kharif_sorghum_production_1000_tons,
       rabi_sorghum_production_1000_tons,sorghum_production_1000_tons,
       pearl_millet_production_1000_tons,maize_area_1000_ha,
       maize_production_1000_tons,maize_yield_kg_per_ha,
       finger_millet_production_1000_tons,groundnut_area_1000_ha,
       groundnut_production_1000_tons,sunflower_area_1000_ha,
       sunflower_production_1000_tons,soyabean_area_1000_ha,
       soyabean_production_1000_tons,soyabean_yield_kg_per_ha,
       oilseeds_area_1000_ha,oilseeds_production_1000_tons,
       sugarcane_production_1000_tons, cotton_production_1000_tons
  
2. Data Collection and Cleaning: Here on going through the existing dataset the cleaning was done based on the fields that are required for the EDA process and the rest of the fields were removed from the dataset.
3. EDA WorkflowThe analysis follows these key steps:
 A. Data Cleaning
 B. Outlier Detection & RemovalWe utilized the Interquartile Range (IQR) method to handle extreme values.Reasoning: Large agricultural districts often appear as outliers compared to smaller ones.Method:
 C. Correlation AnalysisUsed a heatmap to visualize the relationship between numerical variables.
 D. Feature EngineeringYield Calculation: Created a new metric: $\text{Yield} = \frac{\text{Production}}{\text{Area}}$ to measure productivity per hectare.
4. Key VisualizationsBoxplots: To identify outliers in land size and total harvest.Heatmaps: To find hidden correlations between seasonal rainfall and production.Bar Charts: Top 10 rice-producing states in India.Scatter Plots: Area vs. Production to visualize yield efficiency.
5. Major Findings
Finding 1: Rice production is heavily skewed towards 3-4 major states (e.g., West Bengal, Uttar Pradesh).
Finding 2: A strong positive correlation exists between Area and Production, but yield varies significantly by region.
6. Libraries Used:
   Pandas: Data manipulation.
   Matplotlib & Seaborn: Data visualization.
   Numpy: Mathematical operations and outlier masking.

Sql Queries:
For all the given scenarios the SQL queries are written and visualized using Power BI.

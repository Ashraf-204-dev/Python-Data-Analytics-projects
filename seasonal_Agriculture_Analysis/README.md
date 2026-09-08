# 🌾 Seasonal Agriculture Analysis
## 📊 Project Overview

Seasonal Agriculture Analysis is a Python-based data analytics project that analyzes agricultural performance across different seasons, states, crops, environmental conditions, resource usage, production costs, revenue, profit, and water consumption.

The project uses Pandas, NumPy, Matplotlib, and Seaborn to perform data exploration, data-quality analysis, KPI calculation, aggregation, and visualization.

A comprehensive dashboard was created to present important agricultural performance indicators such as:

Average crop yield by season
Average crop yield by state
Average revenue distribution by season
Crop yield vs. water usage

The objective of this project is to transform raw agricultural data into meaningful insights that can help understand seasonal performance, geographical differences, resource utilization, and agricultural profitability.

## 🎯 Objectives

The main objectives of this project are:

Analyze agricultural performance across different seasons.
Compare crop yields across different Indian states.
Examine agricultural revenue and profitability.
Analyze the relationship between crop yield and water usage.
Calculate important agricultural KPIs.
Identify missing and duplicate values in the dataset.
Understand environmental and soil-related factors affecting agricultural production.
Create meaningful visualizations for easier interpretation of agricultural data.
Develop a comprehensive agricultural performance dashboard.
Demonstrate practical Exploratory Data Analysis (EDA) skills using Python.
🗂️ Dataset Information

## The project uses the dataset:

seasonal_agriculture_performance_dataset.csv

Dataset Size
Attribute	Value
Total Records	4,000
Total Columns	28
States	8
Districts	10
Crops	8
Seasons	3
Irrigation Methods	4
States Included
Andhra Pradesh
Gujarat
Karnataka
Madhya Pradesh
Maharashtra
Punjab
Tamil Nadu
Telangana
Crops Included
Wheat
Maize
Pulses
Rice
Cotton
Chilli
Groundnut
Sugarcane
Seasons Included
Kharif
Rabi
Zaid
Irrigation Methods
Drip
Flood
Rainfed
Sprinkler
📋 Dataset Features

The dataset contains agricultural, environmental, financial, and resource-related attributes.

Column	Description
Farm_ID	Unique identifier for each farm
State	State where the farm is located
District	District associated with the farm
Crop	Crop cultivated
Season	Agricultural season
Farm_Area_Hectares	Farm area in hectares
Rainfall_mm	Rainfall received in millimeters
Avg_Temperature_C	Average temperature in Celsius
Humidity_pct	Humidity percentage
Sunlight_Hours_Day	Average daily sunlight
Soil_pH	Soil pH value
Soil_Moisture_pct	Soil moisture percentage
Nitrogen_kg_ha	Nitrogen quantity per hectare
Phosphorus_kg_ha	Phosphorus quantity per hectare
Potassium_kg_ha	Potassium quantity per hectare
Irrigation_Method	Irrigation method used
Fertilizer_kg_ha	Fertilizer quantity per hectare
Pesticide_Litre_ha	Pesticide usage per hectare
Seed_Quality_Score	Seed quality score
Yield_Tonnes_Ha	Crop yield per hectare
Production_Tonnes	Total crop production
Market_Price_INR_Tonne	Market price per tonne
Total_Cost_INR	Total agricultural cost
Revenue_INR	Revenue generated
Profit_INR	Profit or loss generated
Water_Used_m3	Water consumed in cubic meters
Water_Efficiency_t_per_1000m3	Water efficiency
Disease_Pest_Risk_pct	Disease and pest risk percentage
🛠️ Technologies Used
Python
Jupyter Notebook
Pandas
NumPy
Matplotlib
Seaborn

## 🔄 Project Workflow
Raw Agricultural Dataset
          ↓
     Data Loading
          ↓
   Data Exploration
          ↓
   Dataset Information
          ↓
     Data Types
          ↓
   Statistical Analysis
          ↓
 Duplicate Value Check
          ↓
 Missing Value Analysis
          ↓
 Missing Value Treatment
          ↓
      KPI Creation
          ↓
 Data Aggregation
          ↓
   Data Visualization
          ↓
 Agricultural Dashboard
          ↓
      Insights
      
## 🔍 Exploratory Data Analysis
1. Data Loading

The dataset is loaded into a Pandas DataFrame using:

df = pd.read_csv("seasonal_agriculture_performance_dataset.csv")

The first and last records are inspected using:

df.head(10)
df.tail(10)

This provides an initial understanding of the dataset structure and values.

2. Dataset Metadata

The project examines the number of rows and columns using:

print("No.of Rows:", df.shape[0])
print("No.of Columns:", df.shape[1])

The dataset contains:

4,000 rows × 28 columns

3. Data Types

The data types of all columns are examined using:

df.dtypes

The dataset contains both:

Numerical variables
Categorical variables

This distinction is important for performing appropriate analysis and preprocessing.

4. Statistical Analysis

Descriptive statistics are generated using:

df.describe().T

## Important numerical variables analyzed include:

Farm area
Rainfall
Temperature
Soil pH
Fertilizer usage
Crop yield
Production
Market price
Cost
Revenue
Profit
Water usage
Water efficiency

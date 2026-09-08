🌾 Seasonal Agriculture Analysis
📊 Project Overview

Seasonal Agriculture Analysis is a Python-based data analytics project that analyzes agricultural performance across different seasons, states, crops, environmental conditions, resource usage, production costs, revenue, profit, and water consumption.

The project uses Pandas, NumPy, Matplotlib, and Seaborn to perform data exploration, data-quality analysis, KPI calculation, aggregation, and visualization.

A comprehensive dashboard was created to present important agricultural performance indicators such as:

Average crop yield by season
Average crop yield by state
Average revenue distribution by season
Crop yield vs. water usage

The objective of this project is to transform raw agricultural data into meaningful insights that can help understand seasonal performance, geographical differences, resource utilization, and agricultural profitability.

🎯 Objectives

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

The project uses the dataset:

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
🔄 Project Workflow
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
🔍 Exploratory Data Analysis
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

This provides information such as:

Count
Mean
Standard deviation
Minimum
25th percentile
Median
75th percentile
Maximum

Important numerical variables analyzed include:

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
🧹 Data Cleaning
Duplicate Value Analysis

Duplicate records are checked using:

duplicate_count = df.duplicated().sum()

The dataset contains:

0 duplicate records

This means no duplicate rows were identified during the analysis.

Missing Value Analysis

Missing values are identified using:

missing = pd.DataFrame({
    'Missing Count': df.isna().sum(),
    'Missing %': (df.isna().mean() * 100).round(2)
})

print(missing)

Missing values were identified in selected numerical variables, including:

Rainfall_mm
Soil_Moisture_pct
Yield_Tonnes_Ha

Categorical missing values are handled by replacing them with:

Unknown

using:

categorical_columns = df.select_dtypes(include='object').columns

for col in categorical_columns:
    df[col] = df[col].fillna('Unknown')

The notebook specifically applies this treatment to categorical columns. Numerical missing values are not imputed in the current analysis.

📌 Key Performance Indicators (KPIs)
💰 Net Profit / Loss

The total net profit or loss across the dataset is calculated using:

net_profit_loss = df['Profit_INR'].sum()

The calculated total is approximately:

₹446.23 Million

This KPI provides an overall view of the financial performance represented in the dataset.

💵 Cost per Hectare

Cost efficiency is calculated using:

df['Cost_Per_Hectare'] = (
    df['Total_Cost_INR'] / df['Farm_Area_Hectares']
)

This KPI represents the agricultural cost associated with each hectare of cultivated land.

💰 Revenue per Hectare

Revenue efficiency is calculated using:

df['Revenue_Per_Hectare'] = (
    df['Revenue_INR'] / df['Farm_Area_Hectares']
)

This allows agricultural revenue to be compared relative to farm size.

📊 Data Visualization

The project uses Seaborn and Matplotlib to create multiple visualizations.

🌱 1. Average Crop Yield by Season

A bar chart compares average crop yield across:

Kharif
Rabi
Zaid

The analysis shows that:

Season	Average Yield (Tonnes/Hectare)
Kharif	~5.64
Rabi	~5.08
Zaid	~4.67

Kharif has the highest average crop yield among the three seasons represented in the dataset.

🗺️ 2. Average Crop Yield by State

A line chart compares average crop yield across the eight states.

The analysis gives approximately:

State	Average Yield
Punjab	6.12
Karnataka	5.73
Gujarat	5.70
Telangana	5.08
Madhya Pradesh	5.03
Maharashtra	5.03
Tamil Nadu	4.90
Andhra Pradesh	4.65

Punjab records the highest average yield in the analyzed dataset, while Andhra Pradesh records the lowest among the states included.

💰 3. Average Revenue Distribution by Season

A pie chart represents the distribution of average revenue across the three seasons.

Approximate distribution shown in the dashboard:

Kharif: 38.8%
Rabi: 32.8%
Zaid: 28.3%

Kharif contributes the largest share of the average revenue represented in this visualization.

💧 4. Crop Yield vs. Water Used

A scatter plot is created to examine:

Water Used (m³)
        vs.
Crop Yield (Tonnes/Hectare)

This visualization helps investigate how crop yield varies across different levels of water consumption.

The dataset contains a wide range of water usage and yield values. The current notebook uses the scatter plot for visual exploration; it does not calculate a formal correlation coefficient.

📈 Comprehensive Agricultural Performance Dashboard

The project combines multiple visualizations into a single dashboard titled:

Comprehensive Agricultural Performance Dashboard

The dashboard contains four major components:

1. Average Crop Yield by Season

Shows seasonal differences in agricultural productivity.

2. Average Crop Yield by State

Compares agricultural productivity across different states.

3. Average Revenue Distribution by Season

Shows the relative contribution of each season to the average revenue visualization.

4. Crop Yield vs. Water Used

Explores the relationship between agricultural productivity and water consumption.

🖼️ Dashboard Preview

Add the provided dashboard screenshot to your GitHub repository as:

dashboard.png

Then use:

![Comprehensive Agricultural Performance Dashboard](dashboard.png)

The dashboard provides a compact visual summary of seasonal, geographical, financial, and resource-related agricultural performance.

🔎 Key Insights

Based on the analysis performed in the notebook:

🌾 Seasonal Performance
Kharif has the highest average crop yield at approximately 5.64 tonnes/hectare.
Rabi has an average yield of approximately 5.08 tonnes/hectare.
Zaid has the lowest average yield at approximately 4.67 tonnes/hectare.
🗺️ State Performance
Punjab has the highest average crop yield at approximately 6.12 tonnes/hectare.
Karnataka follows with approximately 5.73 tonnes/hectare.
Gujarat has approximately 5.70 tonnes/hectare.
Andhra Pradesh has the lowest average among the eight analyzed states at approximately 4.65 tonnes/hectare.
💰 Revenue

The average revenue visualization shows:

Kharif – approximately 38.8%
Rabi – approximately 32.8%
Zaid – approximately 28.3%
💧 Water Usage

Water consumption varies considerably across the farms, providing an opportunity to investigate water-use efficiency and its relationship with agricultural yield.

💵 Profitability

The total Profit_INR across the dataset is approximately:

₹446.23 Million

The dataset contains both positive and negative profit values, allowing profitability differences between farms to be explored.

📚 Skills Demonstrated

This project demonstrates practical skills in:

Python Programming
Data loading
Data manipulation
Data aggregation
Calculated columns
Basic analytical programming
Pandas
DataFrame operations
Data inspection
Missing-value analysis
Duplicate detection
GroupBy aggregation
Descriptive statistics
NumPy
Numerical data analysis
Supporting analytical operations
Matplotlib
Figure creation
Plot customization
Dashboard layouts
Labels and titles
Seaborn
Statistical visualization
Bar plots
Line plots
Scatter plots
Histograms
Dashboard visualization
Data Analytics
Exploratory Data Analysis
KPI development
Data-quality checking
Trend comparison
Geographical comparison
Resource analysis
Financial analysis
💡 Business / Agricultural Questions Explored

This project can be used to investigate questions such as:

Which season provides the highest average crop yield?
Which state has the highest agricultural productivity?
Which season contributes the highest average revenue?
How does water consumption vary among farms?
How does crop yield vary with water usage?
What is the cost incurred per hectare?
What is the revenue generated per hectare?
Which farms generate losses?
How do environmental variables vary across agricultural records?
Can agricultural resource usage be optimized?
Which states or seasons may require additional productivity analysis?
How can water efficiency be improved while maintaining crop yield?
📁 Project Structure
Seasonal-Agriculture-Analysis/
│
├── Seasonal_Agriculture_Analysis.ipynb
├── seasonal_agriculture_performance_dataset.csv
├── dashboard.png
└── README.md
▶️ How to Run the Project
1. Clone the Repository
git clone https://github.com/your-username/Seasonal-Agriculture-Analysis.git
2. Navigate to the Project Directory
cd Seasonal-Agriculture-Analysis
3. Install Required Libraries
pip install pandas numpy matplotlib seaborn jupyter
4. Open Jupyter Notebook
jupyter notebook
5. Open the Notebook

Open:

Seasonal_Agriculture_Analysis.ipynb
6. Update the Dataset Path

Change the CSV path in the notebook to the location of your dataset:

df = pd.read_csv("seasonal_agriculture_performance_dataset.csv")
7. Run All Cells

Execute the notebook cells sequentially to reproduce:

Data exploration
Data-quality analysis
KPI calculations
Aggregations
Visualizations
Comprehensive dashboard
🚀 Future Enhancements

The project can be further improved by adding:

Interactive dashboards using Power BI
Interactive dashboards using Plotly
Crop-wise yield comparison
Crop-wise profitability analysis
State-wise profit analysis
Irrigation-method comparison
Water-efficiency analysis
Correlation heatmaps
Soil parameter analysis
Rainfall vs. yield analysis
Temperature vs. yield analysis
Fertilizer vs. yield analysis
Machine Learning-based yield prediction
Crop recommendation systems
Profit prediction models
Outlier detection and treatment
Advanced statistical analysis
🎓 Project Type

Project Category: Data Analytics / Exploratory Data Analysis

Domain: Agriculture & Data Analytics

Primary Tools: Python, Pandas, NumPy, Matplotlib, Seaborn

Dataset Size: 4,000 records × 28 columns

👨‍💻 Author

Ashraf Ali

B.Tech – Electrical & Electronics Engineering
Minor – Computer Science & Engineering (AI & ML)

Interested in:

Data Analytics
Python
SQL
Excel
Power BI
Data Visualization
Machine Learning
📌 Conclusion

The Seasonal Agriculture Analysis project demonstrates how Python-based data analytics can be applied to agricultural datasets to understand crop productivity, seasonal performance, state-wise variations, revenue, profitability, and water usage.

Through data cleaning, statistical analysis, KPI calculation, aggregation, and visualization, the project converts raw agricultural records into a structured analytical view.

The Comprehensive Agricultural Performance Dashboard provides a concise way to interpret the major findings and demonstrates practical skills in Python, Pandas, Seaborn, Matplotlib, and Exploratory Data Analysis.

⚠️ Disclaimer

This project is intended for educational and analytical purposes. The insights are based on the supplied dataset and should not be treated as agricultural recommendations without additional domain-specific validation.

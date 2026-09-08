<div align="center">

# 🌾 Seasonal Agriculture Analysis

### 📊 Comprehensive Agricultural Performance Analysis & Dashboard

<p>
  <b>Python • Pandas • NumPy • Matplotlib • Seaborn • Jupyter Notebook</b>
</p>

<p>
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white">
  <img src="https://img.shields.io/badge/NumPy-Analysis-013243?style=for-the-badge&logo=numpy&logoColor=white">
  <img src="https://img.shields.io/badge/Matplotlib-Visualization-orange?style=for-the-badge">
  <img src="https://img.shields.io/badge/Seaborn-Visualization-4C72B0?style=for-the-badge">
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white">
</p>

</div>

---

## 📌 Project Overview

<b>Seasonal Agriculture Analysis</b> is a Python-based data analytics project developed to analyze agricultural performance across different <b>seasons, states, crops, environmental conditions, resource usage, production costs, revenue, profit, and water consumption</b>.

The project performs <b>Exploratory Data Analysis (EDA)</b>, data-quality checks, statistical analysis, KPI calculations, aggregation, and visualization using Python.

A comprehensive dashboard was developed to visually represent important agricultural indicators such as:

<ul>
<li>🌱 Average Crop Yield by Season</li>
<li>🗺️ Average Crop Yield by State</li>
<li>💰 Average Revenue Distribution by Season</li>
<li>💧 Crop Yield vs. Water Used</li>
</ul>

The goal is to convert raw agricultural data into meaningful insights that can help understand <b>agricultural productivity, seasonal variations, geographical performance, profitability, and resource utilization</b>.

---

## 🎯 Objectives

<ul>
<li>Analyze agricultural performance across different seasons.</li>
<li>Compare crop yields across different states.</li>
<li>Analyze agricultural revenue and profitability.</li>
<li>Study the relationship between crop yield and water usage.</li>
<li>Calculate important agricultural KPIs.</li>
<li>Identify duplicate and missing values.</li>
<li>Analyze environmental and soil-related agricultural factors.</li>
<li>Create meaningful data visualizations.</li>
<li>Develop a comprehensive agricultural performance dashboard.</li>
<li>Demonstrate practical Python-based data analytics and EDA skills.</li>
</ul>

---

## 📊 Dataset Overview

<table align="center">
<tr>
<th>Attribute</th>
<th>Value</th>
</tr>

<tr>
<td><b>Total Records</b></td>
<td>4,000</td>
</tr>

<tr>
<td><b>Total Columns</b></td>
<td>28</td>
</tr>

<tr>
<td><b>States</b></td>
<td>8</td>
</tr>

<tr>
<td><b>Districts</b></td>
<td>10</td>
</tr>

<tr>
<td><b>Crops</b></td>
<td>8</td>
</tr>

<tr>
<td><b>Seasons</b></td>
<td>3</td>
</tr>

<tr>
<td><b>Irrigation Methods</b></td>
<td>4</td>
</tr>

</table>

### 🗺️ States

<p align="center">
Andhra Pradesh • Gujarat • Karnataka • Madhya Pradesh • Maharashtra • Punjab • Tamil Nadu • Telangana
</p>

### 🌱 Crops

<p align="center">
Wheat • Maize • Pulses • Rice • Cotton • Chilli • Groundnut • Sugarcane
</p>

### 🌦️ Seasons

<p align="center">
Kharif • Rabi • Zaid
</p>

### 💧 Irrigation Methods

<p align="center">
Drip • Flood • Rainfed • Sprinkler
</p>

---

## 🧾 Dataset Features

<table>
<thead>
<tr>
<th>Column</th>
<th>Description</th>
</tr>
</thead>

<tbody>

<tr><td><code>Farm_ID</code></td><td>Unique identifier for each farm</td></tr>
<tr><td><code>State</code></td><td>State where the farm is located</td></tr>
<tr><td><code>District</code></td><td>District associated with the farm</td></tr>
<tr><td><code>Crop</code></td><td>Crop cultivated</td></tr>
<tr><td><code>Season</code></td><td>Agricultural season</td></tr>
<tr><td><code>Farm_Area_Hectares</code></td><td>Farm area in hectares</td></tr>
<tr><td><code>Rainfall_mm</code></td><td>Rainfall received in millimeters</td></tr>
<tr><td><code>Avg_Temperature_C</code></td><td>Average temperature in Celsius</td></tr>
<tr><td><code>Humidity_pct</code></td><td>Humidity percentage</td></tr>
<tr><td><code>Sunlight_Hours_Day</code></td><td>Average daily sunlight</td></tr>
<tr><td><code>Soil_pH</code></td><td>Soil pH value</td></tr>
<tr><td><code>Soil_Moisture_pct</code></td><td>Soil moisture percentage</td></tr>
<tr><td><code>Nitrogen_kg_ha</code></td><td>Nitrogen quantity per hectare</td></tr>
<tr><td><code>Phosphorus_kg_ha</code></td><td>Phosphorus quantity per hectare</td></tr>
<tr><td><code>Potassium_kg_ha</code></td><td>Potassium quantity per hectare</td></tr>
<tr><td><code>Irrigation_Method</code></td><td>Irrigation method used</td></tr>
<tr><td><code>Fertilizer_kg_ha</code></td><td>Fertilizer quantity per hectare</td></tr>
<tr><td><code>Pesticide_Litre_ha</code></td><td>Pesticide usage per hectare</td></tr>
<tr><td><code>Seed_Quality_Score</code></td><td>Seed quality score</td></tr>
<tr><td><code>Yield_Tonnes_Ha</code></td><td>Crop yield per hectare</td></tr>
<tr><td><code>Production_Tonnes</code></td><td>Total crop production</td></tr>
<tr><td><code>Market_Price_INR_Tonne</code></td><td>Market price per tonne</td></tr>
<tr><td><code>Total_Cost_INR</code></td><td>Total agricultural cost</td></tr>
<tr><td><code>Revenue_INR</code></td><td>Revenue generated</td></tr>
<tr><td><code>Profit_INR</code></td><td>Profit or loss generated</td></tr>
<tr><td><code>Water_Used_m3</code></td><td>Water consumed in cubic meters</td></tr>
<tr><td><code>Water_Efficiency_t_per_1000m3</code></td><td>Water efficiency</td></tr>
<tr><td><code>Disease_Pest_Risk_pct</code></td><td>Disease and pest risk percentage</td></tr>

</tbody>
</table>

---

## 🛠️ Technologies Used

<div align="center">

| Technology          | Purpose                            |
| ------------------- | ---------------------------------- |
| 🐍 Python           | Programming & Data Analysis        |
| 🐼 Pandas           | Data Manipulation & Analysis       |
| 🔢 NumPy            | Numerical Computing                |
| 📊 Matplotlib       | Data Visualization                 |
| 📈 Seaborn          | Statistical Visualization          |
| 📓 Jupyter Notebook | Development & Analysis Environment |

</div>

---

## 🔄 Project Workflow

<div align="center">

```text
Raw Agricultural Dataset
          ↓
     Data Loading
          ↓
   Data Exploration
          ↓
   Dataset Information
          ↓
     Data Cleaning
          ↓
 Duplicate & Missing Value Analysis
          ↓
   Statistical Analysis
          ↓
      KPI Creation
          ↓
 Data Aggregation
          ↓
   Data Visualization
          ↓
 Agricultural Dashboard
          ↓
     Key Insights
```

</div>

---

## 🔍 Exploratory Data Analysis

<details>
<summary><b>1️⃣ Data Loading & Exploration</b></summary>

<br>

The agricultural dataset is loaded into a Pandas DataFrame and examined using functions such as:

```python
df.head()
df.tail()
df.shape
df.info()
df.dtypes
```

These operations provide an initial understanding of the dataset structure, records, columns, and data types.

</details>

<details>
<summary><b>2️⃣ Statistical Analysis</b></summary>

<br>

Descriptive statistics are generated using:

```python
df.describe().T
```

The analysis examines numerical variables including:

<ul>
<li>Farm Area</li>
<li>Rainfall</li>
<li>Temperature</li>
<li>Soil pH</li>
<li>Fertilizer Usage</li>
<li>Crop Yield</li>
<li>Production</li>
<li>Market Price</li>
<li>Total Cost</li>
<li>Revenue</li>
<li>Profit</li>
<li>Water Usage</li>
<li>Water Efficiency</li>
</ul>

</details>

<details>
<summary><b>3️⃣ Data Quality Analysis</b></summary>

<br>

Duplicate values are checked using:

```python
df.duplicated().sum()
```

Missing values are analyzed using:

```python
df.isna().sum()
```

Categorical missing values are handled using an <code>Unknown</code> category where applicable.

</details>

---

# 📌 Key Performance Indicators

## 💰 Net Profit / Loss

The project calculates the total net profit or loss using:

```python
net_profit_loss = df['Profit_INR'].sum()
```

### Total Net Profit

<div align="center">

<h2>₹446.23 Million</h2>

</div>

---

## 💵 Cost per Hectare

Cost efficiency is calculated using:

```python
df['Cost_Per_Hectare'] = (
    df['Total_Cost_INR'] /
    df['Farm_Area_Hectares']
)
```

This provides an estimate of agricultural expenditure per hectare.

---

## 💰 Revenue per Hectare

Revenue efficiency is calculated using:

```python
df['Revenue_Per_Hectare'] = (
    df['Revenue_INR'] /
    df['Farm_Area_Hectares']
)
```

This allows revenue to be evaluated relative to farm size.

---

# 📊 Dashboard

## 🌾 Comprehensive Agricultural Performance Dashboard

<p align="center">
  <img src="dashboard.png" alt="Comprehensive Agricultural Performance Dashboard" width="950">
</p>

The dashboard combines four major visualizations:

<table align="center">
<tr>
<th>Visualization</th>
<th>Purpose</th>
</tr>

<tr>
<td>🌱 Average Crop Yield by Season</td>
<td>Compares agricultural productivity across Kharif, Rabi and Zaid seasons.</td>
</tr>

<tr>
<td>🗺️ Average Crop Yield by State</td>
<td>Compares average agricultural yield across different states.</td>
</tr>

<tr>
<td>💰 Average Revenue Distribution by Season</td>
<td>Shows the relative revenue contribution of different seasons.</td>
</tr>

<tr>
<td>💧 Crop Yield vs. Water Used</td>
<td>Explores the relationship between water consumption and crop yield.</td>
</tr>

</table>

---

# 🌱 Seasonal Yield Analysis

The analysis compares average crop yield across three agricultural seasons.

<table align="center">
<tr>
<th>Season</th>
<th>Average Yield (Tonnes/Hectare)</th>
</tr>

<tr>
<td>🌾 Kharif</td>
<td><b>~5.64</b></td>
</tr>

<tr>
<td>🌱 Rabi</td>
<td>~5.08</td>
</tr>

<tr>
<td>🌿 Zaid</td>
<td>~4.67</td>
</tr>

</table>

<p align="center">
<b>Kharif records the highest average crop yield among the three seasons.</b>
</p>

---

# 🗺️ State-wise Yield Analysis

The average crop yield varies across the eight states included in the dataset.

<table align="center">
<tr>
<th>State</th>
<th>Average Yield</th>
</tr>

<tr><td>Punjab</td><td><b>~6.12</b></td></tr>
<tr><td>Karnataka</td><td>~5.73</td></tr>
<tr><td>Gujarat</td><td>~5.70</td></tr>
<tr><td>Telangana</td><td>~5.08</td></tr>
<tr><td>Madhya Pradesh</td><td>~5.03</td></tr>
<tr><td>Maharashtra</td><td>~5.03</td></tr>
<tr><td>Tamil Nadu</td><td>~4.90</td></tr>
<tr><td>Andhra Pradesh</td><td>~4.65</td></tr>

</table>

<p align="center">
<b>Punjab records the highest average crop yield in the analyzed dataset.</b>
</p>

---

# 💰 Revenue Distribution

The dashboard represents average revenue distribution across the three seasons.

<table align="center">
<tr>
<th>Season</th>
<th>Revenue Share</th>
</tr>

<tr>
<td>🌾 Kharif</td>
<td><b>38.8%</b></td>
</tr>

<tr>
<td>🌱 Rabi</td>
<td><b>32.8%</b></td>
</tr>

<tr>
<td>🌿 Zaid</td>
<td><b>28.3%</b></td>
</tr>

</table>

---

# 💧 Water Usage vs Crop Yield

A scatter plot is used to investigate the relationship between:

<center>

<b>Water Used (m³)</b>

and

<b>Crop Yield (Tonnes/Hectare)</b>

</center>

The visualization helps identify variations in crop yield at different levels of water consumption.

This analysis can provide a foundation for future investigation into:

<ul>
<li>Water-use efficiency</li>
<li>Irrigation optimization</li>
<li>Resource utilization</li>
<li>Sustainable agricultural practices</li>

# 🚗 Car Market Trends Analysis

An exploratory **Car Market Trends Analysis** project using Python and CarDekho data. The project analyzes car listings to understand **car prices, popular car models, yearly distribution, fuel-type price patterns, and overall selling-price trends**.

The analysis is performed using **Jupyter Notebook, Pandas, NumPy, Matplotlib, and Seaborn**, with multiple visualizations combined into a consolidated Car Market Trends Dashboard.

---

## 📌 Project Overview

The automobile market contains a large amount of information related to car models, manufacturing years, prices, fuel types, and other attributes.

This project focuses on analyzing CarDekho car data to identify useful market patterns and trends through **Exploratory Data Analysis (EDA)**.

The analysis covers:

* Dataset structure and dimensions
* Column information
* Statistical analysis
* Duplicate-value detection and removal
* Missing-value analysis
* Average and median selling prices
* Top 10 car models
* Car model distribution across years
* Average present price of popular car models
* Present-price distribution by fuel type
* Comparison between average and median selling prices
* Consolidated visualization dashboard

---

## 🎯 Objectives

The primary objectives of this project are:

1. Analyze the structure and characteristics of the car dataset.
2. Check and improve the quality of the dataset.
3. Identify duplicate records and remove them.
4. Examine missing values in the dataset.
5. Calculate average and median selling prices.
6. Identify the most frequently occurring car models.
7. Analyze the distribution of popular car models across different years.
8. Compare the present prices of the top car models.
9. Study the relationship between fuel type and present price.
10. Visualize important market trends using Python.
11. Build a consolidated dashboard for easier interpretation of results.

---

## 🛠️ Technologies & Libraries

| Technology / Library | Purpose                                           |
| -------------------- | ------------------------------------------------- |
| **Python**           | Main programming language                         |
| **Jupyter Notebook** | Development and analysis environment              |
| **Pandas**           | Data loading, cleaning, manipulation and analysis |
| **NumPy**            | Numerical operations                              |
| **Matplotlib**       | Data visualization                                |
| **Seaborn**          | Statistical visualization                         |
| **Excel**            | Source dataset                                    |

The notebook imports Pandas, NumPy, Matplotlib, and Seaborn for the analysis.

---

## 📂 Project Files

```text
Car-Market-Trends-Analysis/
│
├── Car_Market_Trends_Analysis.ipynb
├── Car Market Trends Analysis with Car Dekho Data.xlsx
└── README.md
```

### 📓 Jupyter Notebook

`Car_Market_Trends_Analysis.ipynb`

Contains the complete Python-based data analysis, data cleaning operations, visualizations, and dashboard.

### 📊 Dataset

`Car Market Trends Analysis with Car Dekho Data.xlsx`

Contains the car-market data used for the analysis.

---

## 🔍 Data Analysis Process

The project follows a structured **Exploratory Data Analysis workflow**.

```text
Raw Car Data
     ↓
Load Dataset
     ↓
Explore Dataset
     ↓
Check Structure & Columns
     ↓
Statistical Analysis
     ↓
Data Quality Check
     ↓
Remove Duplicate Records
     ↓
Analyze Missing Values
     ↓
Price Analysis
     ↓
Car Model Analysis
     ↓
Fuel Type Analysis
     ↓
Data Visualization
     ↓
Car Market Trends Dashboard
```

---

## 🧹 Data Cleaning

Data quality is an important part of the project.

The notebook checks for duplicate records using Pandas and then removes duplicate rows from the dataset.

Missing values are also analyzed by calculating:

* Missing value count
* Missing value percentage

The results are then sorted according to the number of missing values.

---

## 📊 Price Analysis

The project calculates two important statistical measures:

* **Average Selling Price**
* **Median Selling Price**

These values are later compared visually to understand the overall selling-price distribution of the cars.

The notebook calculates the average and median directly from the `Selling_Price` column.

---

## 🚘 Top 10 Car Models Analysis

The project identifies the **10 most frequently occurring car models** using the `Car_Name` column.

The selected models are then analyzed based on their distribution across different manufacturing years.

This helps provide an overview of which car models appear most frequently in the dataset and how their occurrences vary by year.

---

## 📅 Car Model vs Year Analysis

A count plot is used to visualize the distribution of the top 10 car models across different years.

This visualization helps answer questions such as:

* Which models occur most frequently?
* In which years are popular models concentrated?
* How does model availability vary across years?

The notebook filters the dataset to the top 10 car models before creating the visualization.

---

## 💰 Present Price Analysis

The project calculates and visualizes the **average Present Price** for the top 10 car models.

A bar chart is used to compare the average present prices of the selected models.

This analysis can help identify:

* Higher-priced popular models
* Lower-priced popular models
* Differences in market positioning between models

---

## ⛽ Fuel Type Analysis

The project also examines the distribution of **Present Price according to Fuel Type**.

A strip plot is used to visualize the distribution of present prices for different fuel categories.

This provides a visual comparison of car prices across different fuel types represented in the dataset.

---

## 📈 Average vs Median Selling Price

The project compares:

```text
Average Selling Price
        VS
Median Selling Price
```

A bar chart is used to display both values and provide a quick overview of the market's selling-price distribution.

The comparison can also help identify whether the dataset's selling prices may be influenced by relatively high- or low-priced vehicles.

---

# 📊 Car Market Trends Dashboard

The notebook combines four major visualizations into a single **Car Market Trends Dashboard**.

The dashboard contains:

### 1. 📅 Top 10 Models Distribution by Year

Displays the distribution of the top 10 car models across different years.

### 2. 💰 Average Present Price of Top 10 Models

Compares the average present price of the most frequently occurring car models.

### 3. ⛽ Present Price vs Fuel Type

Shows how present prices are distributed across different fuel types.

### 4. 📊 Average vs Median Selling Price

Provides a high-level comparison of the average and median selling prices.

These four visualizations are consolidated into a 2×2 dashboard layout in the notebook.

---

## 💡 Skills Demonstrated

This project demonstrates practical skills in:

### Python

* Variables
* Functions
* Conditional logic
* Data manipulation
* Data visualization

### Pandas

* Reading Excel data
* DataFrame operations
* Duplicate detection
* Duplicate removal
* Missing-value analysis
* Statistical calculations
* Filtering data
* Group-based analysis

### Data Visualization

* Bar charts
* Count plots
* Strip plots
* Dashboard creation
* Comparative visualizations

### Exploratory Data Analysis

* Dataset exploration
* Data-quality assessment
* Descriptive statistics
* Trend identification
* Pattern analysis


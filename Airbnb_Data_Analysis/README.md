# 🏠 Airbnb Data Analytics

An exploratory **Airbnb Data Analytics** project developed using **Python** to analyze Airbnb listing data and uncover patterns related to **property types, locations, pricing, reviews, availability, hosts, and booking characteristics**.

The project uses **Pandas, NumPy, Matplotlib, and Seaborn** to perform data exploration, data-quality checks, data cleaning, statistical analysis, and visualization.

---

## 📌 Project Overview

The Airbnb dataset contains detailed information about property listings, hosts, neighborhoods, prices, reviews, booking preferences, availability, and other listing characteristics.

This project applies an **Exploratory Data Analysis (EDA)** approach to understand the dataset and prepare it for meaningful analysis.

The dataset contains **102,599 rows and 27 columns** before the data-cleaning operations.

The analysis covers important attributes such as:

* Listing ID
* Property name
* Host information
* Host verification
* Neighborhood group
* Neighborhood
* Latitude and longitude
* Country
* Instant booking
* Cancellation policy
* Room type
* Construction year
* Price
* Service fee
* Minimum nights
* Number of reviews
* Last review
* Reviews per month
* Review rating
* Host listing count
* Availability
* House rules
* License information

These columns are explicitly present in the project dataset.

---

## 🎯 Objectives

The main objectives of this project are:

1. Understand the structure of the Airbnb dataset.
2. Explore the available variables and their data types.
3. Perform statistical analysis of numerical and categorical variables.
4. Identify duplicate records.
5. Clean duplicate records from the dataset.
6. Identify missing values and their percentages.
7. Handle missing values in categorical columns.
8. Analyze Airbnb listings based on location and neighborhood.
9. Study room-type distribution.
10. Analyze property pricing patterns.
11. Examine reviews and review ratings.
12. Analyze availability and minimum-night requirements.
13. Generate visualizations to identify meaningful patterns.
14. Develop data-driven insights from Airbnb listing data.

---

## 🛠️ Technologies Used

| Technology / Library                | Purpose                        |
| ----------------------------------- | ------------------------------ |
| **Python**                          | Data analysis and programming  |
| **Jupyter Notebook / Google Colab** | Development environment        |
| **Pandas**                          | Data manipulation and analysis |
| **NumPy**                           | Numerical operations           |
| **Matplotlib**                      | Data visualization             |
| **Seaborn**                         | Statistical visualization      |
| **Microsoft Excel**                 | Source dataset                 |

The notebook imports Pandas, NumPy, Matplotlib, and Seaborn for the analysis.

---

### 📓 `Airbnb_Data_Analytics.ipynb`

Contains the complete Python analysis, including:

* Dataset loading
* Data exploration
* Statistical analysis
* Data-quality checks
* Data cleaning
* Missing-value treatment
* Exploratory analysis
* Visualizations

### 📊 Excel Dataset

`1776250134-P4-Airbnb Hotel Booking Analysis.xlsx`

This is the source dataset used by the notebook.

---

# 🔍 Exploratory Data Analysis

## 1. 📥 Data Loading

The dataset is loaded into a Pandas DataFrame using `read_excel()`.

```python
df = pd.read_excel("1776250134-P4-Airbnb Hotel Booking Analysis.xlsx")
```

The notebook then uses Pandas operations such as `head()`, `tail()`, `shape`, `columns`, and `info()` to understand the dataset.

---

## 2. 📊 Dataset Dimensions

The original dataset contains:

```text
Rows    : 102,599
Columns : 27
```

The notebook obtains this using:

```python
df.shape
```

and records the result as `(102599, 27)`.

---

## 3. 🧾 Dataset Information

The dataset contains a mixture of:

* Integer columns
* Floating-point columns
* Categorical/object columns
* Date/time information

The notebook identifies:

```text
27 total columns
12 float columns
2 integer columns
12 object columns
1 datetime column
```

The `last review` field is stored as a datetime column.

---

# 🧹 Data Cleaning

Data cleaning is an important component of this project.

## Duplicate Records

The project checks the dataset for duplicate rows.

The initial data-quality check identifies:

```text
Duplicate Rows: 541
```

The duplicate records are then removed using:

```python
df = df.drop_duplicates().copy()
```

After cleaning:

```text
Duplicates remaining: 0
```

This ensures that duplicate records do not unnecessarily influence the analysis.

---

## Missing Value Analysis

The project calculates both:

* Missing-value count
* Missing-value percentage

using:

```python
missing = pd.DataFrame({
    'Missing Count': df.isna().sum(),
    'Missing %': (df.isna().mean() * 100).round(2)
})
```

This provides a systematic overview of missing information in every column.

For example, the notebook identifies missing values in fields such as:

* `instant_bookable`
* `last review`
* `review rate number`
* `Column1`

The `Column1` field is particularly incomplete, with the notebook showing **100% missing values** after duplicate removal.

---

## Handling Missing Categorical Data

The project identifies several categorical columns and replaces missing values with:

```text
Unknown
```

The categorical fields include:

```text
NAME
host_identity_verified
host name
neighbourhood group
neighbourhood
country
country code
cancellation_policy
house_rules
```

This is implemented using Pandas `fillna()`.

After filling the categorical missing values, the notebook verifies that these selected columns contain no remaining missing values.

---

# 📈 Statistical Analysis

The project uses:

```python
df.describe(include='all').T
```

to generate descriptive statistics for both numerical and categorical columns.

The statistical analysis provides information such as:

* Count
* Unique values
* Most frequent value
* Frequency
* Mean
* Minimum
* Maximum
* Standard deviation
* Quartiles

For example, the dataset's `price` column has an observed mean of approximately **625.29**, with values ranging from **50 to 1200** in the analyzed data.

---

# 🏘️ Location Analysis

The dataset contains both:

* `neighbourhood group`
* `neighbourhood`

The dataset contains **7 neighborhood groups** and **224 neighborhoods** according to the descriptive analysis.

Geographical coordinates are also available through:

```text
lat
long
```

allowing the dataset to be analyzed spatially.

---

# 🛏️ Room Type Analysis

The `room type` field represents the type of accommodation offered.

The dataset contains **4 distinct room-type categories**, with **Entire home/apt** appearing as the most frequent category in the descriptive statistics.

Room-type analysis can help understand:

* Which accommodation types are most common
* How different room types are distributed
* Potential differences in pricing and availability

---

# 💰 Price Analysis

Price is one of the most important variables in the Airbnb dataset.

The dataset includes:

```text
price
service fee
```

The descriptive statistics show:

| Metric          |  Price |
| --------------- | -----: |
| Mean            | 625.29 |
| Minimum         |     50 |
| 25th Percentile |    340 |
| Median          |    624 |
| 75th Percentile |    913 |
| Maximum         |   1200 |

These values are based on the notebook's statistical output.

Price analysis can be used to explore how accommodation costs vary by:

* Neighborhood
* Room type
* Availability
* Host characteristics
* Other listing attributes

---

# 📋 Important Dataset Variables

| Category      | Variables                                                      |
| ------------- | -------------------------------------------------------------- |
| Listing       | ID, NAME                                                       |
| Host          | Host ID, Host Name, Host Verification                          |
| Location      | Neighborhood Group, Neighborhood, Latitude, Longitude          |
| Booking       | Instant Bookable, Cancellation Policy                          |
| Accommodation | Room Type                                                      |
| Property      | Construction Year                                              |
| Pricing       | Price, Service Fee                                             |
| Stay          | Minimum Nights                                                 |
| Reviews       | Number of Reviews, Last Review, Reviews per Month, Review Rate |
| Availability  | Availability 365                                               |
| Other         | House Rules, License                                           |

These fields are based on the columns available in the uploaded dataset.

---

# 🧠 Data Analytics Workflow

The overall project workflow can be represented as:

```text
Raw Airbnb Dataset
        ↓
Load Excel Dataset
        ↓
Initial Data Exploration
        ↓
Check Rows & Columns
        ↓
Identify Data Types
        ↓
Statistical Analysis
        ↓
Data Quality Check
        ↓
Remove Duplicates
        ↓
Analyze Missing Values
        ↓
Handle Categorical Missing Values
        ↓
Explore Airbnb Attributes
        ↓
Price / Room / Location / Review Analysis
        ↓
Visualization
        ↓
Generate Insights


DashBoard: <a href="https://github.com/Ashraf-204-dev/Python-Data-Analytics-projects/blob/main/Airbnb_Data_Analysis/Screenshot%202026-09-08%20231013.png"> View DashBoard </a>

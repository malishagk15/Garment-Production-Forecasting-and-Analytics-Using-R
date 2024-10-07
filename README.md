# Production Planning Analytics Data

This project focuses on data analysis and machine learning using R programming to process and analyze production planning and actual production data. The primary objective is to build models to forecast actual production based on the planned production data, identify patterns, and provide insightful visualizations.

## Table of Contents
- [Project Overview](#project-overview)
- [Data](#data)
- [Requirements](#requirements)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Preprocessing and Model Building](#preprocessing-and-model-building)
- [Results](#results)
- [Conclusion](#conclusion)
- [References](#references)

## Project Overview
This project analyzes production data from garment factories and applies machine learning techniques to predict actual production based on planned production. Key tasks include:
- Cleaning and preprocessing data.
- Merging planning and actual production datasets.
- Developing machine learning models to forecast production.
- Identifying patterns in production data.
- Visualizing the results.

The dataset includes 6 months of production planning and actual production data from four line sections in a garment factory.

## Data
The data provided consists of 167 CSV files, categorized into two folders:
- **Plan Data**: 49 files representing production plans for 4 line sections (LC Sec 1, LC Sec 2, LC Sec 3, and LC Sec 4).
- **Production Quantities**: 118 files representing actual production data for the same period.

### Key Attributes:
- **Sales Order (S/O)** and **Line Item (LI)** serve as unique keys.
- **SMV (Standard Minute Value)**: Represents the standard time required to complete a product.
- **Efficiency**: Calculated as `Efficiency = Standard Hours / Work Hours`.

## Requirements
The following libraries are required for this project:

```R
library(ggplot2)
library(dplyr)
library(tidyr)
library(caret)
library(randomForest)
```

## Exploratory Data Analysis
The [Exploratory Data Analysis (EDA)](Exploratory_Data_Analysis.html) explores the key patterns in the dataset, including:
- Descriptive statistics of production data.
- Data visualization for planned vs. actual production.
- Identifying outliers and missing values.

The full R Markdown file for EDA can be found [here](Exploratory_Data_Analysis.Rmd).

## Preprocessing and Model Building
The [Preprocessing and Model Building](Preprocessing_And_Model_Building.nb.html) step includes:
1. **Data Cleaning**: Handling outliers, missing values, and normalizing the data.
2. **Dataset Merging**: Combining planned and actual production datasets.
3. **Feature Engineering**: Creating relevant features for machine learning models.
4. **Machine Learning Models**: Applying and comparing models like Random Forest, Decision Trees, and Linear Regression.
5. **Model Evaluation**: Assessing model performance based on accuracy, RMSE, and other metrics.

The full R Markdown file for preprocessing and model building can be found [here](Preprocessing_And_Model_Building.Rmd).

## Results
- **Model Performance**: The models built were evaluated based on accuracy in predicting actual production from the planned data.
- **Patterns Identified**: Various production patterns, including seasonality, sales order trends, and inefficiencies across line sections, were identified.
- **Visualizations**: Key visualizations, such as efficiency over time and production trends, are available in the EDA and model building reports.

## Conclusion
This project provides valuable insights into production planning analytics, enabling better decision-making in a garment factory setting. By predicting actual production based on planned data and identifying key trends, this analysis can help optimize production schedules and improve efficiency.

## References

- [R Documentation](https://www.rdocumentation.org/)

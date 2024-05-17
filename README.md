# Revenue-Estimation-for-Airbnb-Properties

## Overview

This project aims to predict the revenue for Airbnb properties using a predictive model. The model leverages historical data, exploratory data analysis (EDA), and key feature identification to provide actionable insights for Airbnb hosts.

## Team Members
- Piyush Kakde
- Karan Karnik
- Monika Madugula
- Timothy Samuel

## Table of Contents
- [Overview](#overview)
- [Team Members](#team-members)
- [Project Structure](#project-structure)
- [Data](#data)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Preprocessing](#preprocessing)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Results](#results)
- [Business Application](#business-application)
- [References](#references)

## Project Structure

- **Introduction and Problem Statement**: Outline of the project goals and the importance of revenue prediction for Airbnb hosts.
- **Company Overview**: Background on Airbnb and its global presence.
- **Data Investigation**: Details about the dataset used, including size, structure, and key features.
- **Preprocessing**: Steps taken to clean and prepare the data for modeling.
- **Model Implementation**: Development of various models, including XG Boost and Backward Linear Regression.
- **Business Application**: Practical applications of the model for Airbnb hosts and the company.

## Data

### Dataset
- **Size**: 48711 rows and 95 columns.
- **Missing Values**: Significant missing values in the 'revenue' column.
- **Superhost Evaluation Periods**: Data spans multiple evaluation periods, providing both current and historical performance metrics.

### Key Features
- Property characteristics
- Socio-economic factors
- Geographic features
- Seasonal trends

## Exploratory Data Analysis (EDA)

### Before Preprocessing
- Conducted summary statistics and Chi-square tests to identify important features and relationships.

### After Preprocessing
- Analysis revealed that revenue is closely linked to property characteristics, socio-economic factors, and seasonal trends.

## Preprocessing

### Steps:
1. **Remove Irrelevant Records**: Dropped rows with missing revenue values and duplicated variables.
2. **Handle Missing Values**: Imputed missing values using median and mode imputation.
3. **Outlier Treatment**: Applied flooring and capping method for outlier treatment.
4. **Feature Creation**: Added new features such as 'quarter' and one-hot encoded categorical variables.
5. **Lagged Variables**: Introduced one-period lag for certain features to maintain timeline consistency.

## Modeling

### Initial Approach
- Developed models with a focus on balancing accuracy and interpretability.
- Models tested: XG Boost, Optimized XG Boost, Backward Linear Regression.

### Ensemble Method
- Applied ensemble techniques to improve predictive performance.
- Used grid search optimization for fine-tuning model parameters.

## Evaluation

### Metrics
- **R-squared**: Used to measure the predictive accuracy of the models.

## Results

### Model Performance
- **XG Boost**: R-squared of 0.7124.
- **Optimized XG Boost**: R-squared of 0.7201.
- **Backward Linear Regression**: R-squared of 0.6718.

## Business Application

### Practical Applications
- **Revenue Prediction**: Helps current and future hosts understand potential income from property listings.
- **Investment Decisions**: Provides data-driven insights for property investments or enhancements.
- **Supply and Pricing Optimization**: Enables hosts to price properties effectively and align with market demand.

### Interactive Tool
- Reimagined the "What's My Place Worth?" tool to provide more accurate revenue estimates based on a broader range of features.

## References
- Airbnb interactive tool: [What's My Place Worth?](https://www.airbnb.com/host/homes)
- Airbnb Q3 2023 financial results: [Airbnb Q3 2023 Financial Results](https://news.airbnb.com/airbnb-q3-2023-financial-results/)
- Estimating Revenue: [Community Discussion on Revenue Estimation](https://community.withairbnb.com/t5/Ask-about-your-listing/Estimating-Revenue/m-p/1704423)
- 2023 US AirDNA Outlook Report: [AirDNA Report](https://www.airdna.co/industry-report/2023-us-airdna-outlook-report)

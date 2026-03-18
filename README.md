# Transport for London Cycling Analysis & Bike Demand Forecasting 🚴‍♂️📊

A comprehensive data analysis project exploring Transport for London (TFL) cycling usage patterns from 2021-2023, with machine learning models for bike demand forecasting to support strategic expansion into the short-term rental cycle business.

## 📋 Table of Contents
- [Project Overview](#project-overview)
- [Business Challenge](#business-challenge)
- [Dataset](#dataset)
- [Key Features](#key-features)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Science Use Cases](#data-science-use-cases)
- [Machine Learning Models](#machine-learning-models)
- [Key Findings](#key-findings)
- [Business Recommendations](#business-recommendations)
- [Technologies Used](#technologies-used)

## 🎯 Project Overview

This project provides data-driven insights into cycling usage patterns in London to help determine the feasibility of expanding into the short-term rental cycle business. Through comprehensive exploratory data analysis and advanced forecasting models, we identify usage trends, customer profiles, and operational considerations for strategic decision-making.

## 💼 Business Challenge

A client is considering expanding their business into short-term rental cycles in London. Before investing, they need to understand:
- How people in London use cycling services
- Expected usage patterns and customer profiles
- Operational concerns (reliability, supply chain management)
- Strategic insights for successful market entry

## 📊 Dataset

**Source:** Transport for London (TFL) Cycling Usage Statistics (2021-2023)

**Key Variables:**
- Rental ID
- Bike ID and Bike Model
- Start/End Station IDs and Names
- Start/End Times
- Trip Duration
- Temporal features (hour, day, month, year)

## ✨ Key Features

- **Comprehensive EDA:** In-depth analysis of cycling patterns across temporal and spatial dimensions
- **Demand Forecasting:** Advanced ML models (LSTM, XGBoost, Prophet, SARIMA) for 180-day predictions
- **Station Analysis:** Identification of high-traffic stations and popular routes
- **Customer Segmentation:** Analysis of commuter vs. leisure ride patterns
- **Anomaly Detection:** Identification of unusual usage patterns and outliers
- **Actionable Insights:** Data-driven business recommendations for expansion strategy

## 🔍 Exploratory Data Analysis

### 1. Ride Frequency Analysis
- **Hourly Trends:** Peak usage at 8 AM (morning rush) and 5-7 PM (evening commute)
- **Daily Trends:** Consistent weekday usage with slight dips on Monday & Sunday
- **Monthly Trends:** Peak demand during summer months (June-August), decline in winter (December-February)

### 2. Station Activity Heatmap
- **Top Start/End Station:** Hyde Park Corner, Hyde Park (high tourist activity)
- **Popular Routes:** Short, looped trips within parks indicating recreational and tourist usage

### 3. Rush Hour vs Leisure Rides
- **Rush Hour Definition:** 
  - Morning: 07:00 - 10:00 AM
  - Evening: 16:00 - 19:00 PM
- **Finding:** Leisure rides dominate over commuter rides

### 4. Bike Model Performance
- Classic bikes preferred for longer trips
- PBSC_EBIKE used for shorter, faster trips
- Majority of trips fall within 5-15 minute range

### 5. Seasonal & Yearly Trends
- Peak usage in 2022, decline in 2023
- Clear seasonal patterns with summer peaks
- Strong correlation with weather and policy changes

## 🎲 Data Science Use Cases

1. **Bike Demand Forecasting** ⭐ (Selected)
   - Predict peak and future demand times
   - Optimize fleet allocation and service reliability

2. **Bike Availability Optimization**
   - Ensure even distribution across stations
   - Prevent shortages in high-demand areas

3. **Customer Segmentation**
   - Categorize users based on ride behaviors
   - Enable personalized marketing strategies

4. **Trip Duration Prediction**
   - Estimate ride duration for improved ETA accuracy
   - Optimize station rebalancing

5. **Optimal Station Placement**
   - Identify strategic locations for new stations
   - Maximize accessibility and revenue

6. **Anomaly Detection**
   - Identify suspicious activities (theft, misuse, fraud)
   - Improve security and policy enforcement

## 🤖 Machine Learning Models

### 1. LSTM (Long Short-Term Memory)
**Performance:**
- MAE: 3,084
- RMSE: 4,080
- MAPE: 16.19%
- SMAPE: 14.15%

**Strengths:**
- Best for long-term forecasting (6 months)
- Smoother trend prediction
- Superior seasonality learning
- Most stable predictions

### 2. XGBoost
**Performance:**
- MAE: 4,231
- RMSE: 5,612
- MAPE: 21.06%
- SMAPE: 17.70%

**Strengths:**
- Best for short-term forecasting
- Captures demand fluctuations effectively
- Suitable for short-term variations

### 3. Prophet (Facebook)
**Performance:**
- MAE: 4,177.56
- RMSE: 5,603.70
- MAPE: 17.98%
- SMAPE: 16.48%

**Strengths:**
- Automatic seasonality detection (weekly, monthly, yearly)
- Long-term trend variation handling
- Outlier and missing data adaptability
- No train-test split required

### 4. SARIMA
- Time-series forecasting with seasonal components
- Captures cyclical patterns in demand

**🏆 Selected Model:** LSTM demonstrated the best overall performance with lowest error metrics and superior long-term forecasting capability.

## 📈 Key Findings

### Usage Patterns
- 📌 Peak hours: 8 AM and 5-7 PM
- 📌 Highest demand: Weekdays and summer months
- 📌 Popular location: Hyde Park Corner
- 📌 Trip duration: Most trips 5-15 minutes
- 📌 Ride type: Leisure rides dominate (>50%)

### Seasonal Trends
- ☀️ Summer: Highest demand (June-August)
- ❄️ Winter: Significant decline (December-February)
- 📊 Year-over-year: Peak in 2022, decline in 2023

### Operational Insights
- 🔄 Station rebalancing needed for high-traffic locations
- 🚲 Classic bikes preferred for longer trips
- ⚡ E-bikes used for shorter, faster commutes
- 📍 Tourist hotspots show highest activity

## 💡 Business Recommendations

### 1. Seasonal Fleet Optimization & Dynamic Pricing Strategy

**Recommendation:**
- Increase fleet availability during peak months (spring and summer)
- Reduce surplus inventory in winter to optimize operational costs
- Implement dynamic pricing:
  - Higher rates during peak hours/seasons
  - Discounts during off-peak times
- Launch incentive programs during off-peak hours

**Expected Impact:**
- Balanced demand and improved profitability
- Reduced congestion and improved system efficiency
- Enhanced operational cost management

### 2. Targeted Marketing & Expansion Based on High-Demand Zones

**Recommendation:**
- Target high-demand areas for bike station placement:
  - Business districts
  - Universities
  - Tourist hotspots
- Adopt segmented marketing approach:
  - Commuters: Weekday-focused campaigns
  - Leisure cyclists: Weekend promotions
- Use promotional strategies tailored to each group

**Expected Impact:**
- Maximized engagement and usage
- Improved customer acquisition
- Higher retention rates
- Strategic market penetration

## 🛠️ Technologies Used

- **Programming Language:** Python 3.x
- **Data Analysis:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn, Plotly
- **Machine Learning:** 
  - Scikit-learn
  - TensorFlow/Keras (LSTM)
  - XGBoost
  - Prophet (Facebook)
  - Statsmodels (SARIMA)
- **Presentation:** Microsoft PowerPoint
- **Version Control:** Git



# Bike Share Demand Prediction
![GitHib Logo](https://github.com/Bhushan0097/02.CAPSTONE.ML.REGRESSION-BikeShareDemandPrediction/blob/main/data/BikeShare.png)



## Overview
This repository contains the code and resources for a supervised machine learning project aimed at predicting bike share demand in Seoul, South Korea. The dataset used is `SeoulBikeData.csv`.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Dependencies](#dependencies)
- [ML Model Training and Evaluation](#mL-Model-training-and-evaluation)

- [Results](#results)
- [Conclusion](#conclusion)


## Introduction

Bike share demand prediction is a critical aspect of urban transportation planning. This project focuses on using machine learning techniques to predict bike rental demand in Seoul, aiding in efficient resource allocation and city planning.

## Dataset

The dataset `SeoulBikeData.csv` is included in the  📁 `data` directory. It contains information about bike rentals, including weather conditions, temperature, humidity, and other relevant features.

The `SeoulBikeData.csv` file contains the following columns:

- **Date**: Year-Month-Day
- **Rented Bike count**: Count of bikes rented at each hour
- **Hour**: Hour of the day
- **Temperature**: Temperature in Celsius
- **Humidity**: %
- **Windspeed**: m/s
- **Visibility**: 10m
- **Dew point temperature**: Celsius
- **Solar radiation**: MJ/m2
- **Rainfall**: mm
- **Snowfall**: cm
- **Seasons**: Winter, Spring, Summer, Autumn
- **Holiday**: Holiday/No holiday
- **Functional Day**: NonFunctional/Functional Day

## Dependencies

The project is developed using Python and relies on the following libraries:

- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Documentation

The project involves the following steps: <br>
<ol>
  <li>  Data Cleaning and Preparation </li>
  <li>  Exploratory Data Analysis </li>
  <li>  Visualization and Insights </li>
  <li>  Hypothesis Testing </li>
  <li>  Feature Enginerring & Data Pre-processing </li>
  <li>  ML Model Training , Implementation and Evaluation </li>
</ol>

### Data Cleaning and Preparation
The first step in this project involves cleaning and preparing the data. This includes checking for missing data, removing duplicates, and converting data types. Some of the specific tasks involved in this step include:

- Handling missing data
- Removing duplicates
- Converting data types
- TimeSeries Analysis

### Exploratory Data Analysis
The next step in the project is to conduct exploratory data analysis.
This involves examining the data to understand its distribution, central tendencies, and correlations between variables.

### Hypothesis Testing

Hypothesis testing , a statistical method used to make inferences about a population based on a sample of data. To perform hypothesis testing on the 'SeoulBikeData.csv' dataset, we first  start with a null hypothesis (H0) and an alternative hypothesis (H1), then use statistical tests to determine if there is enough evidence to reject the null hypothesis in favor of the alternative hypothesis.

Below is  general step-by-step guide on to perform hypothesis testing on a dataset like SeoulBikeData.csv:<br>
   <ol>
    <li>  Define the Hypotheses </li>
    <li>  Choose a Significance Level (α)</li>
    <li>  Select the Test </li>
    <li>  Perform the Test</li>
    <li>  Analyze the Results </li>
    <li>  Draw Conclusions </li> 
   </ol>


### Feature Enginerring & Data Pre-processing
<ol>
  <li>Handling Missing Values </li>
<li> Handling Outliers </li>
<li> Label Encoding </li>
<li> Textual Data Preprocessing </li>
<li> Feature Manipulation & Selection </li>
  <li> Data Transformation </li>
<li> Data Scaling </li>
<li> Dimesionality Reduction </li>
<li> Data Splitting </li>
</ol>

### ML Model Training and Evaluation
The dependent variable  is **Rented Bike Count** is a contionus variable. Hence to Regression ML algorithms are used to train the model to predict the depedent variable. <br>
Following are the ML algorithms on which the model is trained
<ol> 
<li> Ridge Regression (Logistic Regression + L2 Regularization ) </li>
<li> Decision Tree Regression </li>
<li> Random Forest Regression </li>
</ol>

### Result

| Model Name    | Train r2_score | Test r2_score  | MAE | MSE   |
| ------------- | ------------- | ------------- | ------------- | ------------- |
Ridge Regression (Base Model)           | 0.5969834427027465 | 0.5611509471571063 | 282.97650291199943 | 132052.40508090574 |
| Ridge Regression + GridSearchCV         | 0.5969815828381584 | 0.5612334108757271 | 282.9539718021544  | 132027.59123590542 |
| Decision Tree Regression                |        1.0         | 0.8453401099843291 | 133.34609878310667 | 49702.985325697926 |
| Decision Tree Regression + GridSearchCV | 0.9480705668434853 | 0.8723154222023835 | 125.69186170892704 | 41033.94031865554  |
| Random Forest Regression                | 0.9881705009991666 | 0.9181275336765233 | 100.85899069434504 | 26311.320872154618 |

### Conclusion

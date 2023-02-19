# Data-Science-on-Bike-Sharing-Dataset
BoomBikes Bike Sharing Prediction - Regression Problem

## Table of contents
* [General info](#general-info)
* [Methodology](#methodology)
* [Technologies](#technologies)

# General info

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic.  BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. 

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. 

The company wants to know:

- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demand
- Based on a variety of weather surveys and people's styles, the service provider has compiled a set of data on the daily demand for bicycles in the US market between 2018 and 2019.

### Columns

- season: Seasons: spring, winter, summer, autumn
- yr: year (2018:0 and 2019:1)
- mnth: Month: 1-12
- holiday: Holiday: 0-No 1-Yes
- weekday: Day of the week: 0-6
- weekday: Day of the week: 0-6
- weathersit: Weathersit: 1-3
- temp: Average Temperature on that day
- atemp: Average A-Temperature on that day
- hum: Humidity
- windspeed: Windspeed
- casual: Casual users
- registered: Registered users
- cnt: Daily users count

# Methodology

For this project, I followed the following steps.

**1. Data understanding:**
The first step performed was to get to know and understand the data chosen for the Regression Problem with Python

**2. EDA:**
In a jupyter notebook, I implemented the EDA and an analysis of response and predictor variables.

**3. Data preparation:**
For the following step, I focus on preparing the data through coding and standardisation of variables. I separated the casual and registered columns to generate models for each type of user, as they behave differently.

**4. Modeling:**
Further, in this step, I develop differetn regression model to predict the number of bike registrations.

**5. Final observations:**
Finally, I compared the different models and select the best model between decision tree and random forest; by analyzing the Root Mean Square Error and the R2.

# Technology:
Project is created with:
*Python: 3.9.13

**Data processing**
- import numpy as np
- import pandas as pd
- import sidetable
- from sklearn.preprocessing import OneHotEncoder

**Statistics**
- from scipy import stats
- import researchpy as rp
- from scipy.stats import levene

**Dates**
- from datetime import datetime
- import calendar

**Graphics**
- import matplotlib.pyplot as plt
- import seaborn as sns

** Shapiro Test**
- from scipy import stats

**Asymmetry**
- from scipy.stats import skew

**Kurtosis**
- from scipy.stats import kurtosistest

**Levene Test**
- from scipy.stats import levene

**Warnings configuration**
- import warnings
- warnings.filterwarnings('ignore')

**Modelado y evaluación**
- from sklearn.model_selection import train_test_split
- from sklearn.tree import DecisionTreeRegressor
- from sklearn.ensemble import RandomForestRegressor
- from sklearn import tree
- from sklearn.metrics import r2_score, mean_squared_error, mean_absolute_error
- from sklearn.model_selection import GridSearchCV

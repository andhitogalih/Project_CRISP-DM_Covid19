# Project_CRISP-DM_Covid19

# METHODOLOGY
* [Business Understanding]
* [Data Understanding]
* [Data Preparation]
* [Data Cleansing]
* [Exploratory Data Analysis]

## Business Understanding
### BACKGROUND
In facing the COVID-19 pandemic, a deep understanding of data is a very valuable asset for various parties, including the government, health institutions and the general public. Data analysis on the Indonesian COVID-19 dataset aims to provide better insight into this pandemic, as well as assist in making effective decisions in dealing with the public health crisis. The COVID-19 dataset in Indonesia is arranged based on time series, national level and provincial level. , also accompanied by demographic data from that location/region. This dataset is a compilation of various open data sources, such as the official government website of the COVID-19 Task Force, the Central Statistics Agency, and the InaCOVID-19 Hub.
By utilizing this dataset, several important things that can be explored are:
1. On what date was the highest number of new COVID 19 cases reported in one day?
2. Which province had the highest number of new cases per day?
3. Which island had the highest number of COVID 19 cases per day?
4. Which province had the highest number of new cases per day? highest daily healing?
5. How Correlates Between New Deaths and New Recovery?


## Data Understanding
COVID-19 data in Indonesia from March 1 2020 - September 16 2022. The dataset consists of 31,822 rows and 38 columns.

DATA SOURCE
https://www.kaggle.com/datasets/hendratno/covid19-indonesia

'Date' : Date reported
'Location ISO Code' : Location code based on ISO standard
'Location' : Location name
'New Cases' : Daily positive cases
'New Deaths' : Daily death cases
'New Daily Recovered' : Daily cure cases
'New Active Cases': Daily active cases
'Total Cases': The accumulative number of positive cases up to the associated time
'Total Deaths': The cumulative number of deaths up to the associated time
‘Total Recovered': The cumulative number of cured cases up to the associated time
'Total Active Cases': The cumulative number of active cases up to the associated time
Location Level': Regional or national location level
‘City or Regency': Name of city or region
'Province' : Name of the province of location
'Country' : Country name of location
'Island' : Name of the main island location
'Time Zone' : Time zone location
'Special Status' : Special status of location
'Total Regencies' : The number of districts within the associated location
'Total Cities' : Number of cities within the associated location
'Total Districts' : Number of subdistricts within the corresponding location
'Total Urban Village' : The number of villages within the associated location
'Total Rural Villages' : Number of villages within the associated location
'Area (km  )' : Area of location in square kilometers
'Population' : The number of populations within a related location
'Population Density' : The population density in a related location (formula = Population / Area)
'Longitude' : Longitude of location
'Latitude' : The latitude of the location
'New Cases per Million' : Formula = (New Cases / Population) x 1,000,000
'Total Cases per Million' : Formula = (Total Cases / Population) x 1,000,000
'Total Deaths per Million' : Formula = (Total Deaths / Population) x 1,000,000
'Case Fatality Rate' : Formula = (Total Deaths / Total Cases) x 100
'Case Recovered Rate' : Formula = (Total Recovered / Total Cases) x 100
'Growth Factor of New Cases': Less than 1 means decreased, 1 means none change, more than 1 means increase (formula = Today New Cases / Yesterday New Cases)
'Growth Factor of New Deaths': Less than 1 means decreased, 1 means none change, more than 1 means increase (formula = Today New Deaths / Yesterday New Deaths)

## Data Preparation
Python Version: 3.11.6
Packages:
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Feature Engine

## Data Cleansing
Drop unneeded columns. The fields that will be dropped are 'Location ISO Code', 'City or Regency', 'Country', 'Continent', 'Time Zone', 'Special Status', 'Total Cities', 'Total Districts', 'Total Regencies', 'Total Urban Villages', 'Total Rural Villages', 'Area (km2)', 'New Cases per Million', 'Total Cases per Million', 'New Deaths per Million', 'Total Deaths per Million', 'Growth Factor of New Cases', and 'Growth Factor of New Deaths'.
Change the 'Date' data type to a datetime data type to avoid errors in time-series sequencing in visualizations.
After cleansing, the dataset now has 20 columns

## Exploratory Data Analysis
1. On what date was the highest number of new COVID 19 cases reported in one day?
2. Which province had the highest number of new cases per day?
3. Which island had the highest number of COVID 19 cases per day?
4. Which province had the highest number of new cases per day? highest daily healing?
5. How Correlates Between New Deaths and New Recovery?
  

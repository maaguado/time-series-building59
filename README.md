# Bachelor Thesis - Energy Demand Prediction and Data Imputation in Buildings using Multivariate Time Series Analysis

## Overview

This repository contains the code and documentation for my Bachelor Thesis project, which focuses on using multivariate time series analysis to predict energy demand and impute missing data in building energy consumption.

## Background

The main goal of this thesis is to improve the understanding and efficiency of building operations for reducing energy use, energy costs, and carbon emissions.

Accurate energy consumption predictions and data imputation are important for effective building energy management and reducing energy waste. Traditional single-variable time series methods may not always provide adequate results for this task, especially when multiple variables are involved in energy consumption. This project explores the use of multivariate time series analysis for improving energy demand prediction and data imputation in buildings.

Unfortunately, due to the large dimensions of the data, we were unable to include it in this repository. The dataset collected from the office building in Berkeley, California, consists of data from over 300 sensors and meters collected over a period of three years. This large amount of data would make it impractical to store it within the repository. However, the data can be obtained from the paper "a three-year dataset supporting research on building energy management and occupancy analytics" (https://www.nature.com/articles/s41597-022-01257-). We encourage interested parties to obtain the data from this source and replicate our analysis.


## Project Description

This project includes the following steps:

- Data Cleaning: The original data cleaning code from the paper was not working as expected, so we developed an algorithm that uses ML techniques to interpolate missing data.
- Exploratory Data Analysis: In this step, we analyzed the variables that we will be using using plots and statistical techniques.
- Time Series Analysis: We studied some of the properties specific to time series, such as decomposition, stationarity, etc.
- Prediction and Evaluation: We experimented with multiple forecast algorithms and techniques, such as ARIMA, Prophet, and LSTM.

## Repository Structure 

The files in this repository are divided into two stages of development to reflect the progress of the project. The project is currently in progress, so the repository status represents a snapshot of its development at different points in time. The repository will continue to be updated as the project progresses, so that it accurately reflects its current status.

* ![IN PROGRESS](https://img.shields.io/badge/-PENDING-yellow): the corresponding notebook is currently being coded
* ![DONE](https://img.shields.io/badge/-DONE-green): the corresponding notebook has been completed, but it may still be subject to modifications in order to improve its structure and documentation.


### Data cleaning

| File Name | Description | Stage |
| --- | --- | --- |
| [Main Cleaning Notebook](https://github.com/maaguado/time-series-building59/blob/main/Data%20Cleaning/data_cleaning.ipynb) | includes initial experiments and final algorithm description and execution in the dataset | ![DONE](https://img.shields.io/badge/-DONE-green) |
| [Experiment Notebook](https://github.com/maaguado/time-series-building59/blob/main/Data%20Cleaning/experimento.ipynb) | includes preliminary experiments for different types of time series and missing data distribution | ![DONE](https://img.shields.io/badge/-DONE-green) |
| [Initial Experiment](https://github.com/maaguado/time-series-building59/tree/main/Data%20Cleaning/experimentos/base) | experiment with artificial missing data from 1 to 10 days, it compares how many information we should consider to train the ML algorithms for the imputation | ![DONE](https://img.shields.io/badge/-DONE-green) |
| [Holes Experiment](https://github.com/maaguado/time-series-building59/tree/main/Data%20Cleaning/experimentos/huecos) | experiment with multiple artificial holes in the data, to test the performance of the ML algorithm vs Prophet with different number of holes | ![DONE](https://img.shields.io/badge/-DONE-green) |
| [End Experiment](https://github.com/maaguado/time-series-building59/tree/main/Data%20Cleaning/experimentos/final) | experiment to test the performance of the ML algorithm vs Prophet when the missing data is really close to the end of the time series | ![DONE](https://img.shields.io/badge/-DONE-green) |





### EDA

| File Name | Description | Stage |
| --- | --- | --- |
| [General EDA](https://github.com/maaguado/time-series-building59/blob/main/EDA/EDA_General.ipynb) | Basic plots and statistic properties of all the variables | ![IN PROGRESS](https://img.shields.io/badge/-PENDING-yellow) |
| [Time Series- Specific EDA](https://github.com/maaguado/time-series-building59/blob/main/EDA/EDA_timeseries.ipynb) | Study of time series properties for the main variable (hvac_N) and study of multivariate time series | ![IN PROGRESS](https://img.shields.io/badge/-PENDING-yellow) |



### Forecast



| File Name | Description | Stage |
| --- | --- | --- |
| [General Models](https://github.com/maaguado/time-series-building59/blob/main/Forecast/models.ipynb) | Univariate ARIMA and Prophet models on the main variable  | ![IN PROGRESS](https://img.shields.io/badge/-PENDING-yellow) |

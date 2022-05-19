# CO2 vs. Temperature Exercise (Databricks)
This repository contains exercises in Databricks that ingests Global Temperature and Global Temperature By Country data from Kaggle and CO2 Emissions data from OWID and transforms it. The goal of this exercise is to teach some basics about data wrangling and Spark with respect to real world questions.

* Which countries are worse-hit (higher temperature anomalies)?
* Which countries are the biggest emitters?
* What are some attempts of ranking “biggest polluters” in a sensible way?

## Data Sources
In order to answer some of the questions of the exercise, we picked open-source data from [Open World in Data (OWID)](https://github.com/owid/owid-datasets/tree/0f47d280d298694c50b82db98daa94cd6e867d2e/datasets/CO2%20emissions%20(Aggregate%20dataset%20(2020))) and [Kaggle](https://www.kaggle.com/berkeleyearth/climate-change-earth-surface-temperature-data).

The specific datasets:
* [CO2 Emissions (2020).csv (OWID)](https://github.com/owid/owid-datasets/blob/0f47d280d298694c50b82db98daa94cd6e867d2e/datasets/CO2%20emissions%20(Aggregate%20dataset%20(2020))/CO2%20emissions%20(Aggregate%20dataset%20(2020)).csv)
* [GlobalLandTemperaturesByCountry (Kaggle)](https://www.kaggle.com/berkeleyearth/climate-change-earth-surface-temperature-data?select=GlobalLandTemperaturesByCountry.csv)
* [GlobalTemperatures.csv (Kaggle)](https://www.kaggle.com/berkeleyearth/climate-change-earth-surface-temperature-data?select=GlobalTemperatures.csv)

## Data Sources (Modified!)
Since the point of this exercise is to learn how to work with data and the datasets from OWID and Kaggle are both too clean and curated, a set of dirtied data is provided.

They can be found at:
* [EmissionsByCountry.csv](https://raw.githubusercontent.com/data-derp/exercise-co2-vs-temperature/master/data-ingestion/input-data/EmissionsByCountry.csv)
* [GlobalTemperatures.csv](https://raw.githubusercontent.com/data-derp/exercise-co2-vs-temperature/master/data-ingestion/input-data/GlobalTemperatures.csv)
* [TemperaturesByCountry.csv](https://raw.githubusercontent.com/data-derp/exercise-co2-vs-temperature/master/data-ingestion/input-data/TemperaturesByCountry.csv)

## Prerequisites
* Basic knowledge of Python
* Basic knowledge of Spark
* [Databricks Community Edition (free) account](#create-a-databricks-community-account)

## Create a Databricks Community Account
1. Navigate the [Databricks Community Login Page](https://community.cloud.databricks.com/)
2. Click Signup

<img src="databricks-signup.png" alt="databricks-signup.png" width="200"/>

3. Fill in your details, click "Get Started For Free"

   <img src="databricks-get-started.png" alt="databricks-get-started.png" width="200"/>

4. **SCROLL TO THE BOTTOM** to create a Community Account

   <img src="databricks-create-account.png" alt="databricks-create-account.png" width="200"/>


## Data Ingestion
1. Clone this repo if you haven't already done so
2. Open [Data Ingestion CO2 vs Temperature.py](./data-ingestion/Data%20Ingestion%20CO2%20vs%20Temperature.py) in [Databricks Community Edition](https://community.cloud.databricks.com/)
![databricks-import](databricks-import.png)
3. Follow instructions, move on to following exercises once all tests pass.
4. Solutions can be found [here](./data-ingestion/Data%20Ingestion%20CO2%20vs%20Temperature%20Solutions.py).

## Data Transformation
1. Clone this repo if you haven't already done so
2. Open [Data Transformation CO2 vs Temperature.py](./data-transformation/Data%20Transformation%20CO2%20vs%20Temperature.py) in [Databricks Community Edition](https://community.cloud.databricks.com/)
   ![databricks-import](databricks-import.png)
3. Follow instructions, move on to following exercises once all tests pass.
4. Solutions can be found [here](./data-transformation/Data%20Transformation%20CO2%20vs%20Temperature%20Solutions.py).

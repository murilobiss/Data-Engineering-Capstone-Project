# Data Engineering Capstone Project

The goal of the project is to build an ETL pipeline in Airflow to stage, transform, and load data from a S3 repository into a Redshift data warehouse. The schema of the data warehouse is designed to facilitate queries on international arrival into the United States. 

## Datasets used

The datasets used are a list of international arrivals (I-94 forms) into the United States, demographics of cities in the US, and a table of US airport codes:


- **I-94 Immigration Data**: This data comes from the US National Tourism and Trade Office available [here](https://travel.trade.gov/research/reports/i94/historical/2016.html). Each row has detailed international arrival information into the United States including visa type, port of arrival, mode of transportation, country of origin, birth year.  There are over 80 million visitors to the US every year or roughly 230,000 visitors per day.

- **U.S. City Demographic Data**: This dataset contains information about the demographics of US cities. The dataset comes from OpenSoft available [here](https://public.opendatasoft.com/explore/dataset/us-cities-demographics/export/). 

- **Airport Code Table**: This dataset is a table of airport codes and corresponding cities. The airport codes are either three-letter IATA or four-letter ICAO codes. It is available [here](https://datahub.io/core/airport-codes#data).

# Project Two

Group Members:  Jeremiah Eugenio, Emilio Guzman, Kristy Le, Samantha Seng, Evelyn Votran


With this project, we wanted to compile a list of top Korean dramas based on ratings and genres.
Data pulled to show top Kdrama ratings and genres from Kaggle.

Combined and cleaned 2 datasets to see relations.<br/>
- Kdrama ratings: https://www.kaggle.com/datasets/iphigeniebera/korean-drama-list-about-740-unique-dramas?select=imdb.csv
- Popular Kdramas genres: https://www.kaggle.com/datasets/iphigeniebera/korean-drama-list-about-740-unique-dramas?select=genres.csv


## Table of Contents
[ETL Mapping Document](https://docs.google.com/spreadsheets/d/1dBTmUnmcMzCcIxrLGsUZXh9b_g1hfsFrgedWhSxD9T0/edit#gid=0)


## Data
- Dataset acquired through Kaggle 
- Used imdb dataset and genres dataset
- Transformations we applied
  - Cleaned data frame and removed users and imdb description
  - Uploaded genre file to kdrama file and cleaned data
  - Deduplication to include Kdrama titles with multiple genres
  - Filtered data rating >= 8 
  - Capitalized genre details
- Included Postgres SQL schemas 
- Mapping document for target table

CREATE TABLE kdrama (<br/>
  kdrama_name VARCHAR,<br/>
  imdb_rating INT,<br/>
  genre VARCHAR<br/>
);<br/>

select * from kdrama

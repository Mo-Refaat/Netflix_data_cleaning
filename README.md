# Netflix Movies Dataset Cleaning Project

## Overview
This project involves cleaning, exploring, and visualizing a Netflix movies and shows dataset. The dataset was scraped from IMDb's top Netflix movies and shows page and is used to demonstrate data cleaning, feature engineering, and basic exploratory data analysis (EDA) in preparation for machine learning tasks such as genre prediction.

## Table of Contents
- [Dataset](#dataset)
- [Project Steps](#project-steps)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Visualization](#visualization)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)
- [Author](#author)
- [License](#license)

## Dataset
- **Source:** [Kaggle - Movies Dataset for Feature Extraction & Prediction](https://www.kaggle.com/datasets/bharatnatrayn/movies-dataset-for-feature-extracion-prediction?resource=download)
- **Records:** 9,999
- **Attributes:** 9

### Attributes
- **MOVIES:** Title of the movie or show
- **YEAR:** Year(s) the movie or show was released
- **GENRE:** Genre(s) of the movie or show
- **RATING:** IMDb fan rating out of 10
- **ONE-LINE:** Short description
- **STARS:** Director, main actors, and actresses
- **VOTES:** Number of votes for the rating
- **RunTime:** Duration in minutes
- **Gross:** Total worldwide earnings (removed during cleaning due to missing data)

## Project Steps
1. **Introduction**: Project motivation and dataset description.
2. **Importing Libraries**: pandas, numpy, matplotlib, seaborn.
3. **Loading the Dataset**: Read the CSV file into a pandas DataFrame.
4. **Initial Exploration**: View head, describe statistics, check for missing values.
5. **Data Cleaning**: Drop unnecessary columns, rename columns, handle duplicates and missing values, split and clean text columns, convert data types, reorder columns, and sort data.
6. **Feature Engineering**: Split 'Main Cast' into 'Director' and 'Actors & Actresses', extract and clean 'Release Year', convert columns to numeric types.
7. **Aggregate Functions**: Calculate total votes, mean fan rating, median release year, and identify movies with highest/lowest ratings.
8. **Visualization**: Correlation heatmap, genre distribution pie chart, scatter matrix, and time series of ratings.

## Data Cleaning
- Dropped columns with insufficient data (e.g., "Gross")
- Renamed columns for clarity
- Split "Main Cast" into "Director" and "Actors & Actresses"
- Removed duplicates and handled missing values
- Cleaned text data (removed unwanted characters)
- Converted data types as needed
- Reordered and sorted columns
- Dropped rows with empty values in key columns

## Exploratory Data Analysis
- Used `describe()` to summarize numerical columns (e.g., Fan Rating, Run Time, Votes, Release Year)
- Checked for missing values and data types
- Compared dataset shape before and after cleaning
- Used aggregate functions: sum, mean, median
- Identified movies with highest and lowest fan ratings
- Sampled movies from the median release year

## Visualization
- **Correlation Heatmap**: Shows relationships between numerical features
- **Genre Distribution Pie Chart**: Top 10 genres and others
- **Scatter Matrix**: Pairwise relationships between numerical features
- **Time Series Plot**: Average movie rating per year

## Technologies Used
- Python (pandas, numpy, matplotlib, seaborn)
- Jupyter Notebook

## How to Run
1. Clone this repository.
2. Ensure you have Python 3.x and the required libraries installed:
   - pandas
   - numpy
   - matplotlib
   - seaborn
3. Place the dataset CSV file in the project directory as `Netflix Dataset.csv`.
4. Open the notebook `Netflix Data Cleaning.ipynb` and run the cells sequentially.

## Contact
- **Email**: [Mohamed Refaat](mailto:morefaat356@gmail.com)

## License
- This project is for educational purposes only.

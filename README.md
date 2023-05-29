# SISE2601 Project data description

## Team Members
- Ron Beiden (206628505)
- Ori Flomin (318156775)

This Markdown file describes the data folder structure and organization. 
Our research is based on two databases of shooting incidents that occurred in New York City 
over the past decade

The features in the data are described below:

#### General Details

| Column Name            | Type   | Description                                                       |
|------------------------|--------|-------------------------------------------------------------------|
| INCIDENT_KEY           | Int    | Randomly generated persistent ID for each arrest                  |
| OCCUR_DATE             | Date   | Exact date of the shooting incident                               |
| OCCUR_TIME             | Chr    | Exact time of the shooting incident                               |
| BORO                   | Chr    | Borough where the shooting incident occurred                      |
| PRECINCT               | Int    | Precinct where the shooting incident occurred                     |
| JURISDICTION_CODE      | Int    | Jurisdiction where the shooting incident occurred                 |
| LOCATION_DESC          | Chr    | Location of the shooting incident                                 |
| STATISTICAL_MURDER_FLAG| lgl    | Indicates if the shooting resulted in the victim's death, counted as a murder |
| PERP_AGE_GROUP         | chr    | Perpetrator's age group within a category                         |
| PERP_SEX               | chr    | Perpetrator's sex description                                     |
| PERP_RACE              | chr    | Perpetrator's race description                                    |
| VIC_AGE_GROUP          | chr    | Victim's age group within a category                              |
| VIC_SEX                | chr    | Victim's sex description                                          |
| VIC_RACE               | chr    | Victim's race description                                         |
| X_COORD_CD             | chr    | Midblock X-coordinate for New York State Plane Coordinate System, Long Island |
| Y_COORD_CD             | chr    | Midblock Y-coordinate for New York State Plane Coordinate System, Long Island Zone |
| Latitude               | chr    | Latitude coordinate for Global Coordinate System, WGS 1984        |
| Longitude              | dbl    | Longitude coordinate for Global Coordinate System, WGS 1984       |


# Data analysis review

#### 1. Loading & Cleaning the Data

-   Load libraries
-   Upload the data
-   Rename columns and delete unrelated lines
-   Select relevant columns by date from 2011-2021
-   Normalize the Age_group feature to be numeric and omitting null values
-   Normalize the OCCUR_TIME feature to be more specific as OCCUR_TIME_HOUR

#### 2. Data Analysis

-   Summary Statistic
-   Initial analysis
-   Visualizations - Explore relationships between the different variables

#### 3. Model fit

-   Splitting data to train and test

-   Set seed

-   Build a multi-class classification random forest model to predict the characteristics and patterns of shooting incidents

-   Fit a model to the training data set


#### 4. Test the Model

- Predict on the testing data set

- Calculation of Confusion Matrix to determine Accuracy, Precision, Recall, and F1 Score

- Calculation of probabilities of characteristics by the model


### Results
The project aims to provide insights into the characteristics and patterns of shooting incidents in New York City. The analysis includes summary statistics, initial analysis findings, and visualizations to explore relationships between variables. Additionally, a multi-class classification random forest model is built to predict incident characteristics and patterns.
# Project 2: Music Preferences Analysis

## Overview

This project demonstrates the workflow of a data analyst, from initial exploration to hypothesis testing. Using a dataset from a music streaming service, the goal was to analyze and compare user behavior in the cities of **Springfield** and **Shelbyville** to validate or reject a hypothesis about their music preferences on different days of the week.

## Objective

Test the following hypothesis:

> **"User activity differs depending on the day of the week and the city."**

## Data

The dataset used was `music_project_en.csv`, containing the following columns:

- **userID**: User identifier
- **Track**: Song title
- **artist**: Artist name
- **genre**: Music genre
- **City**: User's city (Springfield or Shelbyville)
- **time**: Time the song was played
- **Day**: Day of the week

## Methodology and Steps

The project was divided into three main steps:

1. **Data Overview**  
    Initial exploration of the dataset to understand its structure, data types, and possible issues such as missing or duplicate values.

2. **Data Preprocessing**  
    Cleaning and preparing the data for analysis:
    - Renaming columns for a clearer and more consistent pattern
    - Identifying and filling missing values (`NaN`)
    - Checking for and removing duplicate rows

3. **Hypothesis Testing**  
    With the cleaned data, the analysis focused on validating the hypothesis. Data was filtered by city and day of the week, and the count of songs by genre was aggregated to compare preferences between Springfield and Shelbyville on Monday, Wednesday, and Friday.

## Skills and Tools Applied

- **Pandas**: DataFrame manipulation, including:
  - Reading and exploring data
  - Filtering data based on conditions (`df[condition]`)
  - Handling missing values (`.fillna()`)
  - Detecting and removing duplicates (`.duplicated()`, `.drop_duplicates()`)
  - Grouping and aggregating data (`.groupby()`, `.count()`)

## Conclusion

This project served as a practical application of the hypothesis testing process, demonstrating how data preprocessing is essential to ensure reliable analytical results. The analysis allowed for conclusions about the differences and similarities in music consumption between the two cities, partially validating the initial hypothesis.

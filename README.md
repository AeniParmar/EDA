Project Overview

This project performs an exploratory data analysis (EDA) of the Zomato dataset to gain insights into restaurant ratings, country-wise data distribution, and other relevant trends. Additionally, it integrates country information using a second dataset and generates visualizations to enhance understanding.

Dataset Information

Datasets Used:

zomato.csv: Contains details of various restaurants, including ratings, location, and delivery options.

Country-Code.xlsx: Maps country codes to country names.

Key Features in Datasets:

Aggregate rating: Overall restaurant rating.

Rating color: Color code for rating visualization.

Country Code: Identifier for restaurant locations.

Has Online delivery: Indicates if online delivery is available.

City: City where the restaurant is located.
Steps in Analysis


1. Data Loading and Initial Exploration

Load the datasets using pandas.

Display the first few rows of the data using .head().

Check data types, missing values, and statistical summaries using .info(), .describe(), and .isnull().sum().

Visualize missing data using a heatmap.

2. Data Merging

Merge zomato.csv with Country-Code.xlsx on the Country Code column using a left join.

3. Data Visualizations

a. Country-Wise Restaurant Distribution

Create a pie chart for the top three countries with the highest number of restaurants.

b. Rating Analysis

Group data by Aggregate rating, Rating color, and Rating text.

Generate bar plots to analyze the number of ratings per category.

Create a count plot for Rating color.

c. Analysis of Zero Ratings

Identify countries with restaurants having zero ratings.

d. Currency Usage by Country

Group data by Country and Currency to map currencies used in each country.

e. Online Delivery Availability

Analyze countries offering online delivery and display them using value counts.

f. City-Wise Restaurant Distribution

Create a pie chart for the distribution of restaurants across the top five cities.

Observations

Rating Distribution:

Most ratings fall between 2.5 and 3.4 (average category).

A significant number of restaurants are "Not Rated."

Country Analysis:

India has the highest number of restaurants with zero ratings.

Currency Analysis:

Each country uses its own specific currency.

Online Delivery:

Online delivery is available in India and UAE.

City Distribution:

Cities with the highest number of restaurants are visualized in a pie chart.


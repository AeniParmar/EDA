**Project Overview**

This project performs an exploratory data analysis (EDA) of the Zomato dataset to gain insights into restaurant ratings, country-wise data distribution, and other relevant trends. Additionally, it integrates country information using a second dataset and generates visualizations to enhance understanding.


_**Dataset Information**
_
Datasets Used:

zomato.csv: Contains details of various restaurants, including ratings, location, and delivery options.

Country-Code.xlsx: Maps country codes to country names.

Key Features in Datasets:

Aggregate rating: Overall restaurant rating.

Rating color: Color code for rating visualization.

Country Code: Identifier for restaurant locations.

Has Online delivery: Indicates if online delivery is available.

City: City where the restaurant is located.

_**Steps in Analysis**_

**1. Data Loading and Initial Exploration**

Load the datasets using pandas.

Display the first few rows of the data using .head().

Check data types, missing values, and statistical summaries using .info(), .describe(), and .isnull().sum().

Visualize missing data using a heatmap.

**2. Data Merging**

Merge zomato.csv with Country-Code.xlsx on the Country Code column using a left join.

**3. Data Visualizations**

_a. Country-Wise Restaurant Distribution_
Create a pie chart for the top three countries with the highest number of restaurants.

_b. Rating Analysis_
Group data by Aggregate rating, Rating color, and Rating text.
Generate bar plots to analyze the number of ratings per category.
Create a count plot for Rating color.

_c. Analysis of Zero Ratings_

Identify countries with restaurants having zero ratings.

_d. Currency Usage by Country_

Group data by Country and Currency to map currencies used in each country.

_e. Online Delivery Availability_

Analyze countries offering online delivery and display them using value counts.

_f. City-Wise Restaurant Distribution_

Create a pie chart for the distribution of restaurants across the top five cities.

-->>**Observations**

Rating Distribution:
Most ratings fall between 2.5 and 3.4 (average category).
A significant number of restaurants are "Not Rated."

Country Analysis:
India has the highest number of restaurants with zero ratings.

Currency Analysis:
Each country uses its own specific currency.

Online Delivery:
Online delivery is available in India and UAE.

_**-->>Libraries Used**_

**pandas**: For data manipulation and analysis.

**numpy**: For numerical operations.

**matplotlib**: For creating visualizations.

**seaborn**: For statistical data visualization.

-->>How to Run the Code

1.Ensure all required datasets (zomato.csv and Country-Code.xlsx) are in the same directory as the code file.

2.Install necessary Python libraries using:
pip install pandas numpy matplotlib seaborn
3.Run the code in a Jupyter Notebook or Python IDE.

**Future Scope**
Extend the analysis to include restaurant cuisines.
Perform time-series analysis if temporal data is available.
Create a dashboard for interactive exploration of the data.

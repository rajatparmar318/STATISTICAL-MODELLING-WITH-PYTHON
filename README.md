# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
Objective:

The goal of this project is to analyze and integrate data from multiple sources to provide insights into the relationship between bike-sharing infrastructure and local points of interest (POIs). The project will leverage data from the CityBikes API, Foursquare API, and Yelp API to explore the distribution and characteristics of bike stations and various local amenities. By merging these datasets and building a regression model, the project aims to uncover patterns and relationships that could be valuable for urban planning, transportation logistics, and local business insights.

Project Breakdown:

Data Acquisition and Exploration:

CityBikes API: Retrieve and understand bike station data for a selected city, including latitude, longitude, and the number of bikes at each station.
Foursquare API and Yelp API: Gather information on local amenities (restaurants, bars, POIs) around each bike station to compare the coverage and quality of data provided by each API.
Data Integration:

Combine the bike station data with the local POI data obtained from Foursquare and Yelp.
Create comprehensive datasets that include bike station details alongside local amenities data.
Data Visualization:

Use data visualization techniques to explore and understand the distribution of bike stations and the characteristics of nearby POIs.
Visualize the relationship between bike station locations and the density/type of local amenities.

Database Creation:
Design and implement an SQLite database to store the collected data.
Ensure the database structure is optimized for querying and analysis.

Model Building:
Develop a regression model using Python’s statsmodels module to analyze the relationship between the number of bikes at each station and the characteristics of nearby POIs.
Interpret the results to derive actionable insights and understand how local amenities might influence bike station usage.
Explore converting the regression problem into a classification problem.
Develop a conceptual framework for classification and potential approaches for implementation.

## Process
Project Initialization
Select Tools and Technologies: Choose the tools and technologies for data acquisition (APIs), data processing (Python libraries), and database management (SQLite).

Data Acquisition and Exploration
CityBikes API
Understand API Structure: Explore the API documentation to understand endpoints, data structure, and parameters.
Select a City: Choose a city covered by the CityBikes API.
Retrieve Data: Fetch bike station data including latitude, longitude, and number of bikes.
Data Exploration: Inspect the structure and content of the data to ensure it meets project needs.

Foursquare and Yelp APIs
Understand API Structures: Review the documentation for both Foursquare and Yelp APIs to understand how to query for POIs.
Set Up API Keys: Obtain necessary API keys for both services.
Query APIs: Fetch data for local amenities (restaurants, bars, POIs) around each bike station using the latitude and longitude.
Data Exploration: Examine the data from both APIs to compare coverage and quality.

Data Integration and Preparation
Data Merging
Create DataFrames: Parse the JSON responses from the APIs into Pandas DataFrames.
Merge Data: Join bike station data with local POI data to create a comprehensive dataset.

Data Cleaning
Handle Missing Values: Address any missing or incomplete data.
Normalize Data: Standardize formats and units where necessary.
Filter and Refine: Ensure that only relevant data is included in the analysis.

Data Storage
Database Design

Define Schema: Design the structure of the SQLite database (tables, columns, relationships).
Create Database: Implement the SQLite database using the defined schema.

Data Insertion
Populate Database: Insert the cleaned and merged data into the SQLite database.

Data Validation
Verify Integrity: Check that data is accurately stored and retrievable from the database.
Run Queries: Test common queries to ensure database performance and correctness.

Data Visualization
Visualization Design

Select Visualization Tools: Choose libraries such as Matplotlib, Seaborn, or Plotly for visualization.
Design Plots: Create visualizations to explore the distribution of bike stations and POIs.
Visualization Execution

Scatter Plots: Plot bike stations against local POIs to observe spatial relationships.


## Results


Foursquare API:

Coverage: Provided a broad range of categories and a substantial number of amenities. It included various attributes such as ratings, price levels, and categories.
Data Quality: Generally accurate, but sometimes lacked comprehensive reviews or detailed category information for certain POIs.
Limitations: Some categories were missing or less detailed compared to Yelp. The data sometimes appeared outdated.
Yelp API:

Coverage: Offered detailed information about local businesses, including comprehensive reviews, ratings, price ranges, and more specific categories.
Data Quality: High quality with extensive reviews and detailed business attributes. Yelp's data tended to be more complete and richer in terms of user-generated content.
Limitations: The number of results returned was sometimes limited by API restrictions and location accuracy issues.

Comparison Summary

Number of POIs: Yelp generally provided more comprehensive information with a higher number of results compared to Foursquare. However, Foursquare had a more diverse set of categories.
Data Richness: Yelp's data was richer in terms of reviews and detailed business attributes, making it more useful for in-depth analysis of local amenities.
Coverage: Both APIs had good coverage, but Yelp offered more detailed and user-centric information, which might be beneficial for consumer-oriented applications

## Challenges 
Needed more time to learn about new functions and how to apply them. Needed more time to explore the code and make adjustments.

## Future Goals
Added a heatmap for reference, more graphs for comparison.

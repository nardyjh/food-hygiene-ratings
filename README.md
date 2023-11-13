# UK Food Standards Agency Database Analysis

This project involves the analysis of food hygiene ratings data provided by the UK Food Standards Agency. The goal is to assist the editors of a food magazine, "Eat, Safe, Love," in evaluating establishments across the United Kingdom. The analysis is conducted using MongoDB for data storage and Jupyter Notebooks for data manipulation and exploration.

# Project Structure
The project is organized into three main parts:

## Part 1: Database and Jupyter Notebook Set Up
The Jupyter notebook NoSQL_setup_starter.ipynb is used to import data from the establishments.json file into MongoDB.
The notebook confirms the creation of the uk_food database and the establishments collection.
Basic data checks and a sample document display are included.

## Part 2: Update the Database
The notebook continues with the update of the database by adding a new halal restaurant, "Penang Flavours" to the establishments collection.
BusinessTypeID for "Restaurant/Cafe/Canteen" is found and used to update the new restaurant.
Unwanted establishments in Dover are removed.
Data types for latitude, longitude, and RatingValue are appropriately converted.

## Part 3: Exploratory Analysis
The Jupyter notebook NoSQL_analysis_starter.ipynb explores specific questions provided by "Eat Safe, Love" using MongoDB queries.
Questions include identifying establishments with a hygiene score of 20, those in London with a RatingValue greater than or equal to 4, the top 5 establishments with a RatingValue of 5 sorted by lowest hygiene score, and the number of establishments in each Local Authority area with a hygiene score of 0.

# Usage
To reproduce the analysis, follow these steps:

## Clone the repository:
git clone https://github.com/nardyjh/nosql-challenge.git
cd nosql-challenge

## Install the required dependencies:
pip install pymongo pandas

## Run the Jupyter notebooks:
Open and run NoSQL_setup_starter.ipynb to set up the database.
Open and run NoSQL_analysis_starter.ipynb to perform exploratory analysis.

# Requirements
MongoDB installed on your local machine or accessible server.
Python 3.x installed with Jupyter Notebooks.
Internet connection for package installations.

# Conclusion
This project provides a comprehensive analysis of food hygiene ratings data, offering valuable insights for decision-making by "Eat, Safe, Love." The organized structure allows for easy reproduction and extension of the analysis. Further improvements and contributions are welcome. 

# Author & Acknowledgements
Jorge Nardy
Information provided by University of Toronto. 

# References
UK Food Standards AgencyLinks to an external site. (2022). UK food hygiene rating data API. https://ratings.food.gov.uk/open-data/en-GBLinks to an external site.. Contains public sector information licensed under the Open Government Licence v3.0Links to an external site.
Accessed Sept 9, 2022 and Sept 12, 2022 with the establishment settings as follows: longitude=51.5072, latitude=-0.1276, maxdistancelimit=4567, pagesize=10000, sortoptionkey=distance, pagenumber=(1,2,3,4,5,6,7,8).
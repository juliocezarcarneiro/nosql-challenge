# nosql-challenge

## Overview
This project focuses on building an ETL (Extract, Transform, Load) pipeline using Python, Pandas, and PostgreSQL. The goal is to extract data from Excel files, transform it into structured DataFrames, and load it into a PostgreSQL database. The project demonstrates skills in data extraction, cleaning, transformation, and database management.

## Table of Contents
1. Overview
2. Project Tasks
3. Key Features
4. Technologies Used
5. Setup Instructions
6. Steps to Reproduce the Project
7. Project Structure
8. References

## Project Tasks
* Part 1: Database and Jupyter Notebook Set Up
    * Imported the establishments.json dataset into MongoDB

    * Created a database named uk_food with collection establishments

    * Verified database creation and document structure

    * Established connection using PyMongo

* Part 2: Update the Database
    * Added New Restaurant:

    * Inserted "Penang Flavours" (halal restaurant in Greenwich)

    * Updated with correct BusinessTypeID

    * Data Cleaning:

        * Removed all establishments in Dover (unwanted jurisdiction)

        * Converted data types:

            * latitude/longitude to decimal numbers

            * RatingValue to integers (converting non-numeric values to nulls)

* Part 3: Exploratory Analysis
    * Performed analysis to answer key questions:

        * Establishments with hygiene score = 20 (worst hygiene)

        * Highly-rated London establishments (RatingValue ≥ 4)

        * Top-rated establishments near Penang Flavours (RatingValue = 5, sorted by hygiene)

        * Local Authorities with most establishments scoring 0 hygiene (best hygiene)

## Key Features
* MongoDB Aggregation Pipelines

* Geospatial Queries

* Data Type Conversion

* Regex Filtering

* Pandas Integration

## Technologies Used
MongoDB (noSQL Database): store and query the dataset

Python: programming language

PyMongo: database connection

Pandas: data manipulation and analysis

pprint (Pretty Print): JSON autputs for better readability

Jupyter Notebook: environment for the projects's development

## Setup Instructions
* Clone this repository: git clone https://github.com//nosql-challenge.git

* Ensure you have MongoDB installed and running

* Import the dataset: mongoimport --db uk_food --collection establishments --file Resources/establishments.json --jsonArray

## Steps to Reproduce the Project
* Run the Jupyter notebooks in order:

    * NoSQL_setup_starter.ipynb (Database Setup)

    * noSQL_analysis_starter.ipynb (Analysis)

## Project Structure

## Project Structure
The repository is organized as follows:

## /noSQL-challenge

- **ETL_Mini_Project_JCarneiro.ipynb**
- **LICENSE.txt**
- **README.md**
- **NoSQL_setup_starter.ipynb**
- **NoSQL_analysis_starter.ipynb**

- **/Resources**:
  - **establishments.json**

## References
* PyMongo: MongoDB, PyMongo Documentation. Retrieved from https://pymongo.readthedocs.io/en/stable/

* Pandas: Powerful data structures for data analysis. Retrieved from https://pandas.pydata.org/docs/

* pprint: Data pretty printer. Retrieved from https://docs.python.org/3/library/pprint.html

* MongoDB: Aggregation Pipelines. Retrieved from https://www.mongodb.com/docs/manual/core/aggregation-pipeline/

* MongoDB: Geospatial Queries in MongoDB. Retrieved from https://www.mongodb.com/docs/manual/geospatial-queries/

* ChatGPT – Assisted with project guidance

* Python: Python Software Foundation. Retrieved from https://docs.python.org/3/
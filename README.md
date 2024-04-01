# Database_Schema_Analysis_and_Query_Prediction

# Assignment: Database Schema Analysis and Query Prediction

## Objective

The goal of this assignment is to fetch a specific MySQL sample database schema from GitHub, load it into a database system, generate and execute a large number of random queries, and analyze these queries to identify unused tables and perform data type validation. Additionally, the historical log of executed queries will be used to train a machine learning model to predict upcoming queries.

## Task 1: Database Setup and Schema Loading

### Fetch Schema
Download the MySQL sample database schema from the given GitHub URL: [mysql-sample-db](https://github.com/mysql/mysql-samples).

### Database Creation
Choose a suitable database system (e.g., MySQL, PostgreSQL) and create a new database instance.

### Load Schema
Load the downloaded SQL schema into your database instance by executing the SQL commands in the `.sql` file. This will create tables and relationships as defined in the schema.

## Task 2: Query Generation and Execution

### Random Query Generation
Develop a script (in Python, JavaScript, or any language of your choice) that can automatically generate a wide variety of SQL queries. These queries should include a mix of SELECT, INSERT, UPDATE, and DELETE operations across the various tables in the database.

### Query Execution
Use the script to execute at least 50,000 queries against your database instance. Ensure that the queries vary significantly and cover all the tables and fields in the database schema.

## Task 3: Logging and Analysis

### Query Logging
Log all executed queries, along with their execution times and outcomes (success or failure), in a structured format (e.g., CSV, JSON).

### Analysis for Unused Tables
Analyze the query logs to identify any tables that were not accessed by any of the queries. Report these as potentially unused tables.

### Data Type Validation
Perform an analysis to check if the data types used in the queries match the data types defined in the database schema. Identify any mismatches or potential issues.

## Task 4: Machine Learning Model for Query Prediction

### Data Preparation
Preprocess the historical log of executed queries to serve as training data for the machine learning model. This may involve feature extraction, normalization, and splitting the data into training and test sets.

### Model Training
Select a suitable machine learning algorithm (e.g., LSTM, Transformer-based models for sequence prediction) to train a model capable of predicting future queries based on the historical data.

### Evaluation
Evaluate the model's performance using appropriate metrics (e.g., accuracy, precision, recall) on the test set. Adjust the model as necessary to improve performance.

### Prediction
Demonstrate the model's capability by using it to predict a set of upcoming queries. Analyze the predictions to understand the model's strengths and weaknesses.


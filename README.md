# Disaster-Response-Pipelines

## Motivation

The goal of this project is to build a machine learning pipeline and productionize the model by leveraging data engineering and machine learning skills.

## Description

### Data
   1. message.csv: A csv file which contains four columns (id, message, original, genre)
   
   2. categories.csv: A csv file which contains two columns (id, categories)
   
   3. DisasterResponse.db: A table which contains processed data in the sqlite database
   
### Script
   1. process_data.py: ETL pipeline
   
   2. train_classifier.py: Machine learning pipeline
   
### App
   1. run.py: Web Application
   
   2. templates: HTML files

## Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

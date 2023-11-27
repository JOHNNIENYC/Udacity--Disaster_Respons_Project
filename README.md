
# Disaster Response Pipeline Project

### Project description

The goal of the project is to build a model for an API to classify disaster messages. Two Datasets "messages" and "categories"are provided. 

The project have three components: 1) ETL Pipeline 2) ML Pipeline 3) Flask Web App

1. ETL Pipeline
    *Loads the messages and categories datasets
    Merges the two datasets
    Cleans the data
    Stores it in a SQLite database
2. ML Pipeline
3. Flask Web App
   
   

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Go to `app` directory: `cd app`

3. Run web app: `python run.py`

4. Click the `PREVIEW` button to open the homepage

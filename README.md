
# Disaster Response Pipeline Project

### Project description

The goal of the project is to build a model for an API to classify disaster messages. Two Datasets "messages" and "categories"are provided by Udacity. 

The project have three components: 1) ETL Pipeline 2) ML Pipeline 3) Flask Web App. The ETL pipeline will read the datasets, clean the data and store in a SQLite database. The ML pipeline will split the previous stored data into training set and a test set. By training the training set using NLTK, scikit-learn package, and gridsearch, a final model using for predicting classification is produced and the model is saved as a pickle file. The Flask web app will be used for displaying the model results.  

1. ETL Pipeline
    * Loads the messages and categories datasets
    * Merges the two datasets
    * Cleans the data
    * Stores it in a SQLite database

2. ML Pipeline
    * Loads data from the SQLite database
    * Splits the dataset into training and test sets
    * Builds a text processing and machine learning pipeline
    * Trains and tunes a model using GridSearchCV
    * Outputs results on the test set
    * Exports the final model as a pickle file
      
3. Flask Web App
    * Modify file paths for database and model as needed
    * Add data visualizations using Plotly in the web app
      
### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Go to `app` directory: `cd app`

3. Run web app: `python run.py`

4. Click the `PREVIEW` button to open the homepage

# ETL-ML-Pipeline

Project to classify messages that are received during disasters & emergency.
The project is part of Udacity's DS Nano Degree program where data is provided by Figure Eight. There are 36 pre-defined
categories for classyfying the messages.

We first build a Data Pipeline which takes the text as input, and identifies the categories (from the pre-defined 36) 
for each message and saves this as a table to a SQL database.

Then we build a Machine Learning pipeline which loads the data, cleans/tokenizes the message text using 
NLTK library and builds a Optimal Random Forest Classifier using Gridsearch.
The precision-recall and F1 score are evaluated and the model is saved.

The project runs in Udacity's IDE. The Jupyternotbooks are saved in this Repo as reference.


Following lines directly provided by Udacity to Run the Pipeline and see results in WebApp:

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

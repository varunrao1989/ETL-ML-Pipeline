# ETL-ML-Pipeline

Project to classify messages that are received during disasters & emergency.
The project is part of Udacity's DS Nano Degree program where data is provided by Figure Eight. There are 36 pre-defined
categories for classyfying the messages.

We first build a Data Pipeline which takes the text as input, and identifies the categories (from the pre-defined 36) 
for each message and saves this as a table to a SQL database.

Then we build a Machine Learning pipeline which loads the data, cleans/tokenizes the message text using 
NLTK library and builds a Optimal Random Forest Classifier using Gridsearch.
The precision-recall and F1 score are evaluated and the model is saved.



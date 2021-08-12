# Sentiment Analysis of Rotten Tomatoes movie reviews

# Overview
  Rotten Tomatoes is an American review-aggregation website for film and television. The company was launched in August 1998 by three undergraduate students at the University of California, Berkeley: Senh Duong, Patrick Y. Lee, and Stephen Wang. Although the name "Rotten Tomatoes" connects to the practice of audiences throwing rotten tomatoes when disapproving of a poor stage performance, the original inspiration comes from a scene featuring tomatoes in the Canadian film Léolo (1992).
  The movies are usually categorized based on Tomato meter rankings.
  
# Problem Statement
  Our project aims at building an end-to-end AI model which does Sentiment Analysis of Rotten Tomatoes movie reviews.
  
# Objectives:
  1.	Our sole objective is to classify the movie review as either rotten or fresh.
  2.	Extensive EDA of reviews.
  3.	Selecting and building powerful models and comparing the outcomes.
  4.	Using the model to classify the reviews.

# Data Set Source
  * https://drive.google.com/file/d/1w1TsJBgmIkZ28d1j7sf1sqcPmHXw352/view

# Files overview
  * Final_Project_AI_Enterprise.ipynb
    * EDA has been performed on the dataset.
    * TF-IDF vectorizer has been used to generate data that can be fed to the machine.
    * Fitted all total of 3 algorithms (Naive bayes, Passive Aggressive Classifier, Logistic Regression).
    * Dumped all the necessary .pkl files of the objects (tfidf, tokenizer) and models (all).
  * flask_rotten_tomatos.py.py
    * This file has the API code using flask.
    * It has the routes ("/", "/predict" POST) to handle queries from user.
    * In "/predict" route, it handles users input and performs pre-processing on it.
    * It transforms the preprecessed text into TF-IDF vectors that will be passed to particular model for prediction.
  * requirements.txt
    * All the required libraries are mentioned with the versions.
  * Pickle/model files
    1. tfidf.pkl
    2. naive_bayes.pkl
    3. passive_agressive_classifier.pkl
    4. logistic.pkl
  * Procfile
    * This file has the command to run the application on heroku.

# Liberaries used in the project
  * MatplotLib (https://github.com/matplotlib/matplotlib)
  * NumPy (https://github.com/numpy/numpy)
  * wordcloud (https://github.com/amueller/word_cloud)
  * nltk (https://github.com/nltk/nltk)
  * Flask (https://github.com/pallets/flask)
  * pickleshare (https://github.com/pickleshare/pickleshare)
  * regex (https://github.com/ziishaned/learn-regex)
  * gunicorn (https://github.com/benoitc/gunicorn)
  * pip-tools (https://github.com/jazzband/pip-tools)

* URL of live model:
  * https://rotton-tomatoes-reviews.herokuapp.com/

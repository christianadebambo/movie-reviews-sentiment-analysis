# Movie Reviews Sentiment Analysis

This repository contains code for sentiment analysis of movie reviews using machine learning techniques. The goal is to predict the sentiment (positive or negative) of movie reviews in the test dataset based on the provided IMDB movie reviews.

Dataset taken from [Kaggle](https://www.kaggle.com/competitions/word2vec-nlp-tutorial/overview)

## Prerequisites

Before running the code, ensure that you have the following libraries installed:

- pandas
- BeautifulSoup
- nltk
- scikit-learn

## Code Explanation

The code performs the following steps:

- Imports the necessary libraries for data handling, text preprocessing, feature extraction, classification, and evaluation.
- Loads the labeled and unlabeled movie review datasets.
- Defines a function to preprocess the text by removing HTML tags, non-alphabetic characters, and stopwords.
- Applies text preprocessing to the movie reviews in the datasets.
- Uses the CountVectorizer to convert the preprocessed movie reviews into feature vectors.
- Splits the labeled dataset into training and validation sets for evaluation.
- Builds and evaluates a Multinomial Naive Bayes classifier using the training and validation sets.
- Builds and evaluates a Random Forest classifier using the training and validation sets.
- Combines the predictions from both classifiers using an ensemble approach.
- Generates predictions for the unlabeled movie reviews in the test dataset.
- Saves the predictions in a CSV file named cv-model.csv.

## Results

The code provides the accuracy of the sentiment predictions on the validation set using the ROC AUC score for both the Multinomial Naive Bayes classifier and the Random Forest classifier. It also presents an ensemble approach that combines the predictions from both classifiers. The final predictions for the unlabeled movie reviews in the test dataset are saved in a CSV file.

## Instructions

To run the project code, follow these steps:

- Download the dataset.
- Install the required dependencies mentioned in the Prerequisites section.
- Run the code in a Python environment that supports Jupyter notebooks or execute the code in a Python script.

Note: Adjustments may be required in the code paths to ensure proper loading of the dataset.

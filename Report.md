# Saudi Newspapers Articles Topic Extraction
By: Rawabi Alharbi

## Abstract
The main goal of this project is to create a classification model on Netflix movies and series to predict weather this movie or series is awarded or not.

## Design
The data provided on Github was stored as json files. Therefore, I needed to concat the files to have one large dataset as a dataframe of Arabic articles.
Then I started the preprocessing by removing non-Arabic letters, English numbers, Arabic punctuations, special characters, and newline characters. Then I applyed TF-IDF Vectorizer and I removed the Arabic stop words. After that, I started the Topic Modeling using NMF and LDA. Finally, I choosed the best model and I visualized the results to figure out the topics.


## Data
In this project we used the data from Github (https://github.com/inparallel/SaudiNewsNet). It contains a set of 31,030 Arabic newspaper articles along with metadata, extracted from various online Saudi newspapers.

## Algorithms
we’ve done the data cleaning and removing the nulls and we did some feature engineering by creating new columns, also we transformed the categorical features into label encoder then we split our data and created our baseline model witch was KNN then we wanted to improve the model, we used decision trees and random forest and xgboosted classifier and ensemble stacking and we found that random forest has the best F1 score since it’s our chosen metric because we want to find the tradeoff between recall and precession, then we deployed our model using flask.


## Tools
- Python and Jupyter Notebook
- Numpy and Pandas for data manipulation
- NLTK, tashaphyne, and Farasa for NLP preprocessing
- Sklearn for ML algorithms
- Matplotlib, pyLDAvis and wordcloud for visuializations


## Communication
In addition to the slides and visuals presented, I will be share my work on my github account
* https://github.com/RawabiKhalaf

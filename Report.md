# Saudi Newspapers Articles Topic Extraction
By: Rawabi Alharbi

## Abstract
The main goal of this project is to extract topics from Arabic articles that are extracted from various online Saudi newspapers using NLP and Topic Modeling techniques.

## Design
The data provided on Github was stored as JSON files. Therefore, I needed to concatenate the files to have one large dataset as a data frame of Arabic articles. Then I started the preprocessing by removing non-Arabic letters, English numbers, Arabic punctuations, special characters, and newline characters. Then I applied TF-IDF Vectorizer and I removed the Arabic stop words. After that, I started the Topic Modeling using NMF and LDA. Finally, I chose the best model and I visualized the results to figure out the topics.


## Data
In this project, we used the data from Github (https://github.com/inparallel/SaudiNewsNet). It contains a set of 31,030 Arabic newspaper articles along with metadata, extracted from various online Saudi newspapers.

## Algorithms
In the topic modeling, I have used two algorithms, NMF and LDA.
* NMF
In this algorithm, I tried to tune over a different number of topics. The best number was 5 topics. and it was easy to interpret each topic using Word Cloud visualization.
* LDA
For this algorithm, I tuned the model using GridSearch and the best number was 3 topics. Then, I tried to visualize it using pyLDvis, but the result was not making any sense. Therefore, I conclude that this model can not be used for this problem and this dataset.

## Tools
- Python and Jupyter Notebook
- Numpy and Pandas for data manipulation
- NLTK, tashaphyne, and Farasa for NLP preprocessing
- Sklearn for ML algorithms
- Matplotlib, pyLDAvis and wordcloud for visuializations


## Communication
In addition to the slides and visuals presented, I will share my work on my Github account
* https://github.com/RawabiKhalaf/saudi-newspapers-articles-topic-modeling/blob/main/Source_code.ipynb

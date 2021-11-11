# Saudi Newspapers Articles Topic Extraction
By: Rawabi Alharbi

## Abstract
The main goal of this project is to extract topics from Arabic articles that are extracted from various online Saudi newspapers using NLP and Topic Modeling techniques.

## Design
The data provided on Github was stored as json files. Therefore, I needed to concat the files to have one large dataset as a dataframe of Arabic articles.
Then I started the preprocessing by removing non-Arabic letters, English numbers, Arabic punctuations, special characters, and newline characters. Then I applyed TF-IDF Vectorizer and I removed the Arabic stop words. After that, I started the Topic Modeling using NMF and LDA. Finally, I choosed the best model and I visualized the results to figure out the topics.


## Data
In this project we used the data from Github (https://github.com/inparallel/SaudiNewsNet). It contains a set of 31,030 Arabic newspaper articles along with metadata, extracted from various online Saudi newspapers.

## Algorithms
In the topic modeling I have used two algorithms, NMF and LDA.
* NMF
In this algorithm, I tryed to tune over different number of topics. The best number was 5 topics. and it was easy to interpret each topic using Word Cloud visualization.
* LDA
* For this algorithm, I tunned the model using GridSearch and the best estimater was 3 topics. The, I tryed to visualiza it using pyLDvis, but the result were not making any scens. Therefore, I conclude that this model can not be used fo this problem and this dataset.


## Tools
- Python and Jupyter Notebook
- Numpy and Pandas for data manipulation
- NLTK, tashaphyne, and Farasa for NLP preprocessing
- Sklearn for ML algorithms
- Matplotlib, pyLDAvis and wordcloud for visuializations


## Communication
In addition to the slides and visuals presented, I will be share my work on my github account
* https://github.com/RawabiKhalaf/NLP_Unsupervied_Project/blob/main/NLP_Topic_Modeling_Project.ipynb

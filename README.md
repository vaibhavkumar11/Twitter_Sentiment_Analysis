# Twitter Sentiment Analysis

## V1
This version of sentiment analysis uses Tweepy library to access the Twitter API and uses the TextBlob library to do sentiment analysis on every tweet.
    Using this we can see the positivity and negativity of each tweet, whatever be its topic.

   ### Dependencies :-
   * Tweepy
   * TextBlob

## V2
   This version of sentiment analysis uses the US Airline Tweets Dataset.The tweets are preprocessed and all stop words are removed and words are lematized using WordNet lemmatizer.The sentiment analysis is performed using the TextBlob library with an accuract of 62% on the test set.
   
   ## Dependencies:
   * TextBlob
   * WordNet Lemmatizer
   * NLTK
   
## V3
In this version of sentiment analysis we perform preprocessing on the tweets by removing all stopwords and then WordNet Lemmatizer is used to remove similar words.Then most common 3000 words from training set are found to make the training set.Various Machine Learning models(SVM, Random Forests, Multinomial Naive Bayes) are used from the sklearn library and the best accuracy is found by SVM at 77.6% by tweaking certain parameters.

   ## Dependencies:
   * Sklearn
   * WordNet Lemmatizer
   * NLTK
 
## V4
We have used the IMDB Large Review dataset(preloaded in keras and converted to integer tokens) to perform sentiment analysis.We have 1 LSTM layer and 1 Dense layer(with sigmoid activation) to perform sentiment analysis.This is different from the earlier versions because the average length of reviews in this dataset is 470 words which is much larger than those used in earlier cases.LSTM helps in this case as it remember words from earlier better(to understand about LSTM read chris olah's post about the same). After training we have been able to achieve 83% accuracy after using a single LSTM unit and the first 500 words from vocabulary.

   ## Dependencies:
   * Tensorflow
   * Keras
   * Numpy

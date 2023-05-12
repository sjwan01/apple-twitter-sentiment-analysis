# Twitter Sentiment Analysis

## Background

Natural Language Processing (NLP) focuses on analyzing natural language using text and speech data. It is a field that utilizes techniques from numerous subjects to develop models that could enable computers to understand human language. Applications of NLP include machine translation, text generation, speech recognition, etc., and in this project, we will explore sentiment analysis.

Sentiment analysis aims to determine the emotion behind texts, and it is usually a classification task. It can be done using models that are trained on datasets labeled with sentiment types such as positive, neutral, or negative. Sentiment analysis is useful in a variety of settings. For instance, companies can use sentiment analysis to understand customer opinions on their products and services and thus identify areas to improve.

In this project, we obtain an entity-level sentiment analysis dataset of Twitter. We start with cleaning and transforming the text data into the appropriate format and train several linear models and neural networks, compare and discuss their mechanisms as well as performance and capability to handle text classification tasks in general.

## Data

While the datasets are found on [__*Kaggle*__](https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis), you may also access them in this repository.

They are entity-level sentiment analysis datasets of Twitter. In total, there are about 75k records with 4 features: `Tweet ID`, `entity`, `sentiment`, and `Tweet content`. An overview of the datasets can be found on Kaggle.

In this project, we only make use of text data from `Tweet content` to predict `sentiment` labels.

## Goals

This project is exploratory in nature. In my last semester of college, I took some beginners' courses about [__*recurrent neural networks*__](https://www.udemy.com/certificate/UC-7da07ed7-14ad-4960-ae0f-fc3b8bbc1b46/) and [__*NLP*__](https://www.udemy.com/certificate/UC-534bcbbe-7a7c-4798-8481-551da26b3a1e/) on Udemy and felt genuinely interested. I hope to familiarize myself with common text classification models as well as methods of text preprocessing with some hands-on experience.

The high-level scheme of this project is to develop and experiment with several models that can classify tweets into positive, negative, and neutral sentiment types and, hopefully, identify the most effective approach for sentiment classification of tweets. Give our sample size and my research as well as confidence, the objective is to achieve an accuracy score over 90%.

## Models

The following classification models are trained and evaluated in this project:
- Logistic Regression
- Support Vector Machine
- Bidirectional GRU
- Bidirectional LSTM
- BERT

Logistic regression and support vector machine are linear models, bidirectional GRU and bidirectional LSTM are neural networks, and BERT is based on the transformer architecture. We will evaluate their performance mainly based on their accuracy scores.

# Consumer Sentiment Analysis - Amazon

## Objective

Amazon is an international e-commerce giant with a massive portfolio of products offered online, ranging from electronics to fresh produce. Even though being the pioneer in the e-retail market, it has created a treasure trove of reviews for its products. The goal is to develop an automated text-based classification system that can accurately predict the sentiments of Amazon online consumer reviews. The study focuses on data collected from Amazon.com, consisting of reviews on fine food. The model will take reviews as input and predict whether the review is positive, negative, or neutral.

The dataset used for this project is available at Kaggle: [Amazon Fine Food Reviews](https://www.kaggle.com/snap/amazon-fine-food-reviews).

## Introduction

This project aims to leverage Natural Language Processing (NLP) techniques to analyze consumer sentiments in reviews. By understanding the sentiment behind customer feedback, businesses can improve their products and customer service.

## Dataset

The dataset used in this project is the Amazon Fine Food Reviews dataset, which includes over 500,000 food reviews. Each review consists of the following fields:
- Id
- ProductId
- UserId
- ProfileName
- HelpfulnessNumerator
- HelpfulnessDenominator
- Score
- Time
- Summary
- Text

## Methodology

1. **Data Preprocessing**: Cleaning the text data, removing stop words, and tokenization.
2. **Feature Extraction**: Converting text data into numerical representations using techniques like TF-IDF or word embeddings.
3. **Model Training**: Using machine learning models such as Logistic Regression, Naive Bayes, and advanced models like LSTM for training.
4. **Evaluation**: Assessing model performance using metrics like accuracy, precision, recall, and F1-score.

## Data Pre-processing

Steps taken to clean and preprocess the data:
- Removed null values.
- Dropped unwanted features like `Id` and `ProfileName`.
- Joined `Summary` and `Text` features into a new feature `Summary_Text`.
- Converted Unix timestamps to human-readable dates.
- Calculated a `Helpfulness Ratio`.
- Cleaned the text data by removing punctuation, special characters, and stop words.

## Exploratory Data Analysis

- Distribution of review scores and sentiments.
- Analysis of review length and helpfulness over time.
- Word frequency analysis for positive, negative, and neutral reviews.
- Visualization of top reviewers and their review characteristics.

## Model Building

Three models were built and evaluated:

1. **Multinomial Naive Bayes**:
   - Achieved an accuracy of 78.5%.

2. **Logistic Regression**:
   - Achieved an accuracy of 82.4%.

3. **Long Short-Term Memory (LSTM)**:
   - Achieved an accuracy of 87.2%.
   - Best performing model with the highest accuracy and F1-score.

## Results

The results section includes detailed findings, model performance metrics, and visualizations that highlight the effectiveness of the sentiment analysis models.

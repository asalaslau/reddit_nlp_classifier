# ![](logo.png) Food Delivery Service Analysis on Reddit: UberEats and DoorDash

## Overview

Currently, Too Good To Go does not offer a food delivery service to reach a broader audience while promoting consumption habits that improve society. Last year, we sold a total of 121 million meals. While comparing ourselves to companies like DoorDash, which processes over 2.16 billion delivery orders, may seem ambitious, it is still a possibility.

In this project, we analyze the food ordering and delivery users of Doordash and UberEats on the social media platform Reddit. These two companies account for over 80% of the market. By analyzing their presence on Reddit, we aim to gain insights into customer and delivery driver profiles. In any market, the customer is always right, but in this case, it particularly depends on delivery drivers, who are the face of your company.

**Project Goals**:

* Analyze the differences in posts from DoorDash and UberEats users in specific subreddits to identify key topics and sentiment.
* As a future analysis, explore the distinction between drivers and consumers to better understand the experiences of each user type.

**Problems We Might Encounter**:
* Focusing only on Reddit might affect our ability to obtain a complete picture of what is happening.
* There are other food delivery companies that we are not considering in this study.
* There may be no significant differences between companies on Reddit.

This project utilizes PRAW (Python Reddit API Wrapper) for data collection, focusing on text analysis, and applies Random Forest and Logistic Regression models

## Table of Contents

1. Overview
2. Executive Summary
3. Data
4. Requirements
5. Methods
6. EDA (Exploratory Data Analysis)
7. Data Processing
8. Conclusion & Next Steps
9. Non Course Sources

## Executive Summary

In this project, we explore the user discussions on Reddit regarding UberEats and DoorDash, two dominant players in the food delivery market. By analyzing customer reviews, delivery driver feedback, and general sentiment, we aim to extract valuable insights into their user profiles, satisfaction levels, and common pain points. We focus on text analysis and machine learning models (Random Forest and Logistic Regression) to uncover patterns in user behavior and identify potential differences between the two services.

The data collection from Reddit, using PRAW, offers a rich source of information from real users. This analysis will help Too Good To Go consider how it could adapt and expand into the competitive food delivery market.

## Data

The data used in this project was collected from Reddit using the PRAW API. The dataset includes posts and comments from subreddits discussing UberEats and DoorDash. We specifically focus on:

* Customer reviews of the food delivery services.
* Delivery driver experiences.
* General opinions and feedback on the two platforms.

The data set consists of approximately 2,700 posts. This allows for a comprehensive analysis of user sentiment and feedback for both UberEats and DoorDash. The data is analyzed through text mining techniques, sentiment analysis, and machine learning models to understand the market dynamics and user satisfaction.

## Requirements

To run this project, you will need the following:

- Access to python a to the internet (for collecting data from Reddit)

Python Libraries:
- PRAW: Python Reddit API Wrapper for Reddit data collection
- Pandas: Data manipulation and analysis
- NumPy: Numerical computing
- Matplotlib: Data visualization
- Scikit-learn: Machine learning models and evaluation
- nltk: Natural Language Toolkit for text processing
- Seaborn: Visualization library for statistical data

## Methods

Exploratory Data Analysis (EDA)
Before building the models, we perform Exploratory Data Analysis to understand the structure of the data. Key steps include:

Data Cleaning: Removing duplicates, handling missing values, and cleaning text data.

Text Preprocessing: Tokenization, stemming, and removing stopwords.

Sentiment Analysis: Analyzing the sentiment of posts and comments using text mining techniques.

Feature Engineering: Creating features like word frequency, post length, and sentiment scores.

Data Processing

TF-IDF Vectorization: Text data is transformed into numerical representations using TF-IDF vectorizer.

Model Training: Both Random Forest and Logistic Regression models are trained using the processed data.

Model Evaluation: The models are evaluated using accuracy, classification report, and ROC-AUC to understand their performance.

## Conclusion & Next Steps
We have developed a good model for differentiating between app users based on their posts. However, the results are not fully conclusive, as they heavily depend on the presence of app names in the user's post. These app names serve as key features for classification, which can limit the model's performance when they are absent or ambiguous in the text.

**Next Steps**

* Categorize Posts by Main Subject: To improve classification accuracy, we recommend expanding the analysis by categorizing posts according to their main subject. This will help identify the underlying themes and improve the model's ability to differentiate between app users even in the absence of app names.
* Advanced Text Analysis Techniques: We should explore more advanced techniques in text analysis, such as Natural Language Processing (NLP) methods like topic modeling or sentiment analysis, which can offer deeper insights into the content of user posts.
* Ensemble Learning: To create a more robust model, consider using ensemble learning methods. Combining different models (e.g., decision trees, support vector machines, and neural networks) can increase classification accuracy by leveraging the strengths of each model and reducing the overall error rate.

By implementing these next steps, we can enhance the model's reliability and gain a more comprehensive understanding of user behavior and sentiment across different apps.

## Non-Course Sources 

IBM Machine Learning Documentation: IBM ML Docs

WordClouds.com: WordClouds
These sources can provide valuable insights and tools for enhancing your machine learning models and data visualizations.

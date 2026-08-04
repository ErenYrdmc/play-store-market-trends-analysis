# Google Play Store: Market Trends & Sentiment Analysis

A data science project that analyzes the Google Play Store ecosystem to find out what makes an app successful. This repository covers the entire pipeline from raw data cleaning and exploratory data analysis (EDA) to building a machine learning model for sentiment analysis on user reviews.

## Overview

The mobile app market is highly competitive. To stand out, developers need to understand market gaps and user expectations. In this project, I used Play Store data to answer questions like:
- Which app categories are over-saturated?
- What drives user installations?
- How can we automatically classify user feedback?

## 📂 Dataset

The dataset used in this project is publicly available on Kaggle. You can find the raw data and column descriptions here:
[Google Play Store Apps Dataset by lava18](https://www.kaggle.com/datasets/lava18/google-play-store-apps)

## The Process

**1. Data Cleaning & Preprocessing**
- Handled missing data and duplicates.
- Cleaned string columns (`Installs`, `Price`, `Size`) by stripping characters (`+`, `,`, `$`) and converting them to numeric types.
- Parsed date columns into datetime objects.

**2. Exploratory Data Analysis (EDA)**
- Visualized the distribution of apps across different categories.
- Compared app size vs. user ratings using scatter plots.
- Analyzed market supply versus actual user demand.

**3. Sentiment Analysis (NLP)**
- Used a TF-IDF Vectorizer to process text data from app reviews.
- Trained a Logistic Regression model to classify reviews into positive or negative sentiments.
- Built a custom `predict_sentiment()` function to test raw text inputs in real-time.

## Key Findings

- **The Developer Bias:** There is a huge supply of "Family" apps, but actual user demand doesn't match it. Developers are over-producing in this category.
- **Gaming Dominance:** "Games" rank second in total app count, but they absolutely dominate the market in actual user acquisition (11+ Billion installs).
- **The Monopoly Effect:** Categories like "Communication" and "Video Players" have a relatively low number of apps but account for billions of installs, showing that a few tech giants hold these markets.

## Tech Stack

- **Language:** Python 3
- **Data Manipulation:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-Learn (Logistic Regression, TF-IDF)

## How to Run

1. Clone this repository:
   ```bash
   git clone [https://github.com/ErenYrdmc/play-store-market-trends-analysis.git](https://github.com/ErenYrdmc/play-store-market-trends-analysis.git)

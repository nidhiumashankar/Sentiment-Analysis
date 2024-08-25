# Sentiment-Analysis
The Sentiment Analysis Project focuses on analyzing and classifying text reviews using three different sentiment analysis techniques. It implements Multinomial Naive Bayes, a probabilistic model that classifies text based on a labeled dataset; TextBlob, a library that simplifies sentiment analysis tasks with a user-friendly API; and NLTK’s SentimentIntensityAnalyzer, which uses a rule-based approach for evaluating sentiment scores.

The project involves training a Multinomial Naive Bayes model on a dataset of text reviews and applying both TextBlob and NLTK’s SentimentIntensityAnalyzer to assess sentiment in sample reviews. The goal is to compare the performance of these methods, providing insights into their effectiveness and limitations in sentiment classification.

## Overview

This project demonstrates sentiment analysis using three different algorithms:
1. **Multinomial Naive Bayes**
2. **TextBlob**
3. **NLTK's SentimentIntensityAnalyzer**

The goal is to classify text reviews into positive, negative, or neutral sentiments and compare the results of different sentiment analysis techniques.

## Project Structure

The repository includes the following files:

- `train.csv`: The dataset used for training the Multinomial Naive Bayes model.
- `sentiment_analysis.py`: The main Python script that performs sentiment analysis using the three algorithms.
- `LICENSE`: The MIT License file for the project.
- `README.md`: This README file.

## Installation

To run this project, you'll need to have Python and the following libraries installed:

- pandas
- scikit-learn
- textblob
- nltk

You can install these dependencies using pip:

```bash
pip install pandas scikit-learn textblob nltk
```
Additionally, you'll need to download the necessary NLTK data. You can do this by running the following code in your Python environment:
```bash
import nltk
nltk.download([
    "names",
    "stopwords",
    "state_union",
    "twitter_samples",
    "movie_reviews",
    "averaged_perceptron_tagger",
    "vader_lexicon",
    "punkt",
])
```
## Usage
*Prepare the Dataset*

-Ensure that train.csv is in the same directory as the Python script. The CSV file should have the following format:
```bash
text,label
"I love this product.",positive
"The service was terrible.",negative
```
-Run the Sentiment Analysis

-Execute the Python script sentiment_analysis.py to perform sentiment analysis:

```bash
python sentiment_analysis.py
```
The script will:

- Train a Multinomial Naive Bayes model using the data from train.csv.
- Evaluate sample reviews using the trained model.
- Perform sentiment analysis using TextBlob and NLTK's SentimentIntensityAnalyzer.
- Output the sentiment for each review and the overall sentiment analysis result.
  
## License
This project is licensed under the MIT License. See the LICENSE file for more details.

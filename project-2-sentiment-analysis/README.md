
# Sentiment Analysis Using Natural Language Processing (NLP)

## Project Overview

This project focuses on building a machine learning model that classifies movie reviews as either positive or negative using Natural Language Processing (NLP).

The project explores text preprocessing, feature extraction and machine learning classification techniques.

## Datasets

Two datasets are used:

### 1. Starter Dataset
- File: `sentiment_reviews.csv`
- A small dataset provided as a starting point for understanding the task and developing the initial pipeline.

### 2. IMDb Large Movie Review Dataset
- Contains 50,000 labelled movie reviews.
- 25,000 reviews for training.
- 25,000 reviews for testing.
- Balanced between positive and negative reviews.

Source: https://ai.stanford.edu/~amaas/data/sentiment/

## Technologies and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK
- Scikit-learn
- Jupyter Notebook

## Text Preprocessing

The text preprocessing steps include:

1. Converting text to lowercase.
2. Removing HTML tags.
3. Removing punctuation and special characters.
4. Tokenization.
5. Stopword removal while preserving important negation words.
6. Lemmatization.

## Feature Extraction

TF-IDF (Term Frequency–Inverse Document Frequency) is used to convert text reviews into numerical features that machine learning models can understand.

The vectorizer uses a maximum of 5,000 features.

## Machine Learning Models

The following classification models were trained and evaluated:

- Multinomial Naive Bayes
- Logistic Regression

## Model Evaluation

The models were evaluated using accuracy, precision, recall, F1-score and confusion matrices.

| Model | Accuracy |
|---|---:|
| Multinomial Naive Bayes | 84.08% |
| Logistic Regression | 88.17% |

Logistic Regression achieved the higher accuracy on the test dataset.

## Custom Sentiment Prediction

A `predict_sentiment()` function was developed to classify new movie reviews as:

- Positive Sentiment 😊
- Negative Sentiment 😞

## Project Structure

```text
project-2-sentiment-analysis/
├── README.md
├── requirements.txt
├── sentiment_analysis.ipynb
├── sentiment_analysis_benchmark.ipynb
└── datasets/
    └── sentiment_reviews.csv
    ```

    ## How to Run

    1. Clone or download the repository.
    2. Install the required dependencies using:

       `pip install -r requirements.txt`

       3. Open either notebook in Jupyter Notebook or Google Colab.
       4. Run the notebook cells sequentially.

       The IMDb dataset can be downloaded from the Stanford source linked above.

       ## Objective

       To develop an NLP-based sentiment classification system, understand text preprocessing and feature extraction, and compare the performance of different machine learning classifiers.
       
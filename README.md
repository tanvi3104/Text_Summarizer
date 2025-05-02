# Text Summarizer using Machine Learning

This project is text summarizer that identifies and selects the most important sentences from news articles to generate concise summaries using machine learning models and sentence embeddings.

## Project Overview

The summarizer performs the following steps:
- Splits articles and summaries into individual sentences
- Uses Sentence Transformers to generate semantic embeddings for each sentence
- Labels sentences as 1 if they appear in the reference summary, otherwise 0
- Trains classifiers (e.g., Logistic Regression, SVM) to predict which sentences should be included in a summary
- Builds an extractive summary by selecting the most relevant sentences based on predictions

## Technologies Used

- Python
- scikit-learn
- NLTK
- Sentence Transformers (`all-MiniLM-L6-v2`)
- imbalanced-learn (SMOTE)
- pandas, NumPy

## Dataset

**Note:** The full dataset of news articles and summaries is not included in this repository due to size.

The project was trained on a dataset consisting of:
- News articles stored as `.txt` files
- Human-written summaries stored as `.txt` files with matching filenames

If you would like to run this project, you can:
- Prepare your own dataset with a similar structure
- Or modify the notebook to use a publicly available dataset such as:
  - BBC News Summary Dataset: https://www.kaggle.com/pariza/bbc-news-summary
  - CNN/DailyMail Dataset: https://huggingface.co/datasets/cnn_dailymail

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/text-summarizer-ml.git
   cd text-summarizer-ml

# Amazon-User-Review-Sentiment-Analysis-using-RNNs-Text-classification
# Sentiment Analysis Using RNNs - Project Readme

**Project Title:** Sentiment Analysis Using RNNs

**Date:** 20.09.2023

**Author:** Siyabulela Mathe

**Overview:**

This project focuses on performing sentiment analysis on Amazon product reviews using Recurrent Neural Networks (RNNs). The goal is to classify reviews as positive or negative, providing insights into customer opinions.

**Dataset:**

* **Source:** Amazon product review text data (general appliances) from Jianmo Ni, Jiacheng Li, and Julian McAuley's EMNLP 2019 paper, "Justifying recommendations using distantly-labeled reviews and fined-grained aspects."
* **Format:** Gzipped JSON file (json.gz), extracted using the Windows tar command.
* **Suitability for RNNs:** The dataset is ideal for RNN processing due to the sequential nature of text data. RNNs excel at capturing long-term dependencies and understanding the relationships between words, crucial for accurate sentiment analysis.

**Methodology:**

1.  **Problem Definition:**
    * Understanding the value of product review sentiment analysis for businesses.
    * Exploring how sentiment analysis can improve product development, marketing, and customer experience.

2.  **Data Exploration:**
    * Utilizing PySpark and Apache Spark for data loading and exploration.
    * Addressing challenges encountered with JSON file reading due to PySpark version incompatibility.
    * Focusing on understanding data structure, identifying key features, and handling missing values.

3.  **Data Processing and Preparation:**
    * Employing text processing techniques:
        * Data cleaning (removing noise, punctuation, stop words, etc.).
        * Tokenization/Word Embedding (converting text to numerical format).
        * Feature extraction.

4.  **Model Development:**
    * Setting target (sentiment) and independent (review text) variables.
    * Splitting data into training (80%) and testing (20%) sets to mitigate overfitting and underfitting.
    * Utilizing a word embedding layer with pre-trained GloVe word embeddings.
    * Understanding and implementing GloVe for word representation.

5.  **Model Evaluation:**
    * Evaluating model performance using metrics: accuracy, F1-score, precision, and recall.
    * Visualizing training and validation accuracy/loss using plots.
    * Analyzing plots to identify overfitting/underfitting and guide hyperparameter tuning.

6.  **Model Optimization:**
    * Exploring hyperparameter tuning for the embedding layer.
    * Adjusting parameters: vocabulary length, embedding dimensionality, weights, and input sequence length.
    * Removing unnecessary layers/nodes to prevent overfitting.

**Bibliography:**

1.  Nabi, J. 2018 Machine learning — text Processing, Towards Data Science.
2.  Olsson, F., 2009. A literature survey of active machine learning in the context of natural language processing.
3.  Nigam, V. 2019 Natural language processing: From basics to using RNN and LSTM, Analytics Vidhya.

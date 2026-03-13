# Drug Review Analysis and Classification

This repository contains a machine learning project focused on analyzing and classifying drug reviews from the UCI Machine Learning Repository. The project leverages Natural Language Processing (NLP) to categorize patient feedback across various medical conditions with high precision.

## Project Overview

The core of this project is a classification pipeline designed to predict medical conditions based on the text of patient reviews. By utilizing advanced feature extraction techniques and linear classification models, the system achieves a high degree of accuracy in identifying the context of patient experiences.

## Key Features

* **High-Accuracy Classification:** Achieves **94.0% accuracy** using a Passive Aggressive Classifier.
* **Advanced Text Vectorization:** Implements `TfidfVectorizer` with an `ngram_range` of (1,3), capturing unigrams, bigrams, and trigrams for better contextual understanding.
* **Comprehensive EDA:** Visualizes the distribution of ratings and the most frequent medical conditions.
* **Multi-Class Evaluation:** Detailed performance analysis using confusion matrices for specific conditions including:
    * Birth Control
    * Bipolar Disorder
    * Depression
    * Insomnia
    * Pain
    * Anxiety
    * Acne
    * Weight Loss

## Machine Learning Pipeline

### 1. Feature Engineering
The model uses TF-IDF (Term Frequency-Inverse Document Frequency) weighting. By including trigrams (`ngram_range=(1,3)`), the vectorizer accounts for short phrases and specific medical terminology that single words might miss.

### 2. Model Selection
* **Passive Aggressive Classifier:** This model was selected for its efficiency in large-scale text classification, providing the optimal balance between training speed and predictive power.
* **Multinomial Naive Bayes:** Used as a baseline for comparing classification performance.

### 3. Performance
The optimized model yields the following results:
* **Accuracy:** 0.940
* **Evaluation:** Validated through a confusion matrix to ensure consistent performance across all primary medical categories.



# Fake News Detection using NLP and Machine Learning

## Overview

This project builds a **Fake News Detection system** using **Natural Language Processing (NLP)** and **Machine Learning**. The goal is to classify news articles as **Fake** or **Real** based on their textual content.

The workflow includes **text preprocessing, feature extraction using TF-IDF vectorization, model training with Logistic Regression, and evaluation using standard classification metrics**.

This project demonstrates a complete **machine learning pipeline for text classification**.

---

## Problem Statement

The rapid spread of misinformation on online platforms has made automated fake news detection increasingly important.
This project aims to develop a machine learning model capable of analyzing the text of news articles and predicting whether the news is **fake or legitimate**.

---

## Dataset

The dataset used contains two collections of news articles:

* **Fake.csv** – Fake news articles
* **True.csv** – Real news articles

Each record contains:

* Title
* Text
* Subject
* Date

Dataset Source:
https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset

---

## Technologies Used

* Python
* Pandas
* NumPy
* NLTK (Natural Language Toolkit)
* Scikit-learn
* Matplotlib
* Seaborn
* Google Colab

---

## Project Workflow

### 1. Data Loading

Load fake and real news datasets into Pandas DataFrames.

### 2. Data Labeling

Assign binary labels:

Fake → **0**
Real → **1**

### 3. Data Preprocessing

Text cleaning includes:

* converting text to lowercase
* removing punctuation and numbers
* removing stopwords
* basic normalization of text

### 4. Feature Extraction

Convert textual data into numerical vectors using **TF-IDF Vectorization**.

TF-IDF measures the importance of words in a document relative to the entire dataset.

### 5. Train-Test Split

The dataset is divided into:

* **80% training data**
* **20% testing data**

This allows evaluation on unseen data.

### 6. Model Training

A **Logistic Regression classifier** is trained using the TF-IDF feature vectors.

### 7. Model Evaluation

The model is evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

### 8. Prediction

The trained model can classify new news articles as **Fake** or **Real**.

---

## Model Evaluation

The model performance is evaluated using classification metrics and visualized using a **confusion matrix**.

Example metrics include:

* **Accuracy** – overall correctness of predictions
* **Precision** – reliability of fake news predictions
* **Recall** – ability to detect fake news correctly
* **F1 Score** – balance between precision and recall

---

## Project Structure

```
Fake-News-Detection
│
├── data
│   ├── Fake.csv
│   └── True.csv
│
├── notebook
│   └── Fake_News_Detection.ipynb
│
├── images
│   └── confusion_matrix.png
│
├── requirements.txt
│
└── README.md
```

---

## Installation

Install required libraries:

```
pip install -r requirements.txt
```

---

## Requirements

```
pandas
numpy
matplotlib
seaborn
scikit-learn
nltk
```

---

## Future Improvements

Possible extensions for this project include:

* implementing additional models such as **Naive Bayes or Random Forest**
* experimenting with **word embeddings and deep learning models**
* building a **web application for real-time fake news detection**
* deploying the model using **Flask or FastAPI**

---

## Author

**Jaspreet Kaur**
Computer Science Student | AI & Data Science Enthusiast

This project is part of my ongoing journey to build practical skills in **Machine Learning, NLP, and Data Science through hands-on projects**.

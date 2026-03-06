# Fake News Detection using NLP and Machine Learning

## Overview

This project builds a **Fake News Detection system** using **Natural Language Processing (NLP)** and **Machine Learning** techniques. The objective is to classify news articles as **Fake** or **Real** based on their textual content.

The system processes raw text data, performs preprocessing and cleaning, converts the text into numerical features using **TF-IDF vectorization**, and trains a **Logistic Regression classifier** to detect misinformation.

This project demonstrates a complete **machine learning workflow for text classification**, including preprocessing, feature extraction, model training, and evaluation.

---

## Problem Statement

The rapid spread of misinformation across digital platforms has made automated fake news detection an important challenge. This project aims to build a machine learning model that analyzes the content of news articles and predicts whether the information is **fake or legitimate**.

---

## Dataset

The dataset used for this project contains two types of news articles:

* **Fake.csv** → Fake news articles
* **True.csv** → Real news articles

Each record contains:

* Title
* Text
* Subject
* Date

Dataset source:

https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset

⚠️ The dataset is not included in this repository due to file size limitations.

After downloading the dataset, place the files in a folder named **data**.

Example:

```id="p9e3rn"
Fake-News-Detection
│
├── data
│   ├── Fake.csv
│   └── True.csv
```

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

## Machine Learning Pipeline

### 1. Data Loading

Load the fake and real news datasets into Pandas DataFrames.

### 2. Data Labeling

Assign labels to distinguish between fake and real news:

Fake → **0**
Real → **1**

### 3. Text Preprocessing

Text cleaning includes:

* converting text to lowercase
* removing punctuation and numbers
* removing stopwords using NLTK
* basic text normalization

### 4. Feature Extraction

Text is converted into numerical vectors using **TF-IDF Vectorization**, which measures the importance of words within documents.

### 5. Train-Test Split

The dataset is divided into:

* **80% training data**
* **20% testing data**

This ensures the model is evaluated on unseen data.

### 6. Model Training

A **Logistic Regression classifier** is trained using the TF-IDF features.

### 7. Model Evaluation

Model performance is evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

### 8. Prediction

The trained model can classify new news articles as **Fake** or **Real**.

---

## Model Evaluation

A **confusion matrix** is used to visualize prediction results and identify:

* True Positives
* True Negatives
* False Positives
* False Negatives

This helps understand how accurately the model detects fake news.

---

## Project Structure

```id="72ehm5"
Fake-News-Detection
│
├── notebook
│   └── Fake_News_Detection.ipynb
│
├── images
│   └── confusion_matrix.png
│
├── requirements.txt
│
├── README.md
│
└── .gitignore
```

---

## Installation

Clone the repository:

```id="5f0j2j"
git clone https://github.com/yourusername/Fake-News-Detection.git
```

Install dependencies:

```id="9a3hza"
pip install -r requirements.txt
```

---

## Requirements

```id="evsxeb"
pandas
numpy
matplotlib
seaborn
scikit-learn
nltk
```

---

## How to Run the Project

1. Download the dataset from Kaggle
2. Place **Fake.csv** and **True.csv** inside the `data` folder
3. Install required dependencies
4. Open the notebook and run all cells

---

## Future Improvements

Possible improvements include:

* implementing additional models such as **Naive Bayes or Random Forest**
* experimenting with **word embeddings and deep learning models**
* building a **web interface for real-time fake news detection**
* deploying the model using **Flask or FastAPI**

---

## Author

**Jaspreet Kaur**
Computer Science Student | AI & Data Science Enthusiast


This project is part of my journey to build strong skills in **Machine Learning, Natural Language Processing, and Data Science through hands-on projects**.

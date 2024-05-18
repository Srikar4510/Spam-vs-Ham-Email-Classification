# Spam vs Ham Email Classification

This project aims to classify emails as either spam or ham (not spam) using Natural Language Processing (NLP) techniques and a Logistic Regression model. The dataset contains labeled emails and the goal is to accurately predict the category of new email messages.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Dataset](#dataset)
- [Data Processing](#data-processing)
- [Model Training](#model-training)
- [Model Evaluation](#model-evaluation)
- [Making Predictions](#making-predictions)
- [Results](#results)
- [Requirements](#requirements)
- [Contributing](#contributing)
- [License](#license)

## Introduction

In this project, we use NLP techniques to preprocess email text data and then train a Logistic Regression model to classify emails as spam or ham. 

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Srikar4510/Spam-vs-Ham-Email-Classification.git
    cd Spam-vs-Ham-Email-Classification
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Dataset

The dataset used in this project is a CSV file named `mail_data.csv`, which contains two columns: `Category` and `Message`.

- **Category**: Label of the email (spam or ham)
- **Message**: The text content of the email

## Data Processing

1. Load the dataset into a pandas DataFrame.
2. Replace null values with an empty string.
3. Encode the labels: spam as 0 and ham as 1.
4. Perform text preprocessing:
    - Remove non-alphabetic characters.
    - Convert to lowercase.
    - Remove stopwords.
    - Apply stemming.
5. Split the data into training and testing sets.
6. Convert text data into numerical features using TF-IDF Vectorizer.

## Model Training

1. Train a Logistic Regression model using the training data.

## Model Evaluation

1. Evaluate the model's performance on both training and testing data using accuracy scores.

## Making Predictions

1. Define the input data for prediction.
2. Convert the input text to feature vectors.
3. Use the trained model to predict the label.
4. Output whether the email is ham or spam.

## Results

- **Accuracy on training data**: 97.08%
- **Accuracy on test data**: 96.77%


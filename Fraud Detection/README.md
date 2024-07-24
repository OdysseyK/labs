# Fraud Detection with Decision Tree Classifier

## Overview

This repository contains a machine learning project for detecting fraudulent transactions using a Decision Tree classifier. The project includes data preprocessing, model training, evaluation, and visualization techniques to understand and enhance the model's performance.

## Dataset Features

- **step**: Represents a unit of time where 1 step equals 1 hour.
- **type**: Type of online transaction.
- **amount**: The amount of the transaction.
- **nameOrig**: Customer starting the transaction.
- **oldbalanceOrg**: Balance before the transaction.
- **newbalanceOrig**: Balance after the transaction.
- **nameDest**: Recipient of the transaction.
- **oldbalanceDest**: Initial balance of recipient before the transaction.
- **newbalanceDest**: The new balance of recipient after the transaction.
- **isFraud**: Indicates whether the transaction is fraudulent.

## Results

The Decision Tree classifier has achieved impressive performance on the test dataset:

- **Accuracy**: The model achieved an accuracy score of **0.9997**, indicating that 99.97% of the transactions were correctly classified as either fraudulent or non-fraudulent. This high accuracy demonstrates the model's effectiveness in distinguishing between fraudulent and legitimate transactions.

- **Confusion Matrix**: The confusion matrix reveals the following:
  - **True Positives (TP)**: Correctly identified fraudulent transactions.
  - **True Negatives (TN)**: Correctly identified non-fraudulent transactions.
  - **False Positives (FP)**: Transactions incorrectly identified as fraudulent.
  - **False Negatives (FN)**: Fraudulent transactions incorrectly identified as non-fraudulent.

  The high accuracy score suggests that the classifier has a low rate of both false positives and false negatives, although further inspection of the confusion matrix is recommended for a detailed understanding of model performance.

- **Feature Importance**: The model's decision-making process is influenced by the following features, with their relative importance visualized in the provided charts:

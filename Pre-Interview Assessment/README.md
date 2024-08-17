
# Model Comparison and Evaluation

## Models Tested
1. **Logistic Regression**
2. **Naive Bayes**
3. **K-Nearest Neighbors**

### Features Used
- **Age**: Numerical
- **BusinessTravel**: Categorical (encoded)
- **Education**: Numerical
- **MaritalStatus**: Categorical (encoded)
- **OverTime**: Categorical (encoded)
- **DailyRate**: Numerical
- **Gender**: Categorical (encoded)

### Evaluation Metrics
- **Accuracy**: The proportion of correct predictions.
- **Classification Report**: Precision, recall, F1-score, and support for each class.
- **Confusion Matrix**: Breakdown of actual vs predicted values.

### Model Selection Rationale
- **Logistic Regression**: Chosen for its simplicity and interpretability.
- **Naive Bayes**: Selected for its effectiveness with small datasets and categorical variables.
- **K-Nearest Neighbors**: Picked for its instance-based learning and simplicity.

### Results and Discussion

| Model                 | Accuracy |
|-----------------------|----------|
| Logistic Regression   | 0.91 |
| Naive Bayes           | 0.92 |
| K-Nearest Neighbors   | 0.97 |

#### Logistic Regression
- **Confusion Matrix**: 
[[195, 5], [15, 9]]
- **Classification Report**:
```
              precision    recall  f1-score   support

           0       0.93      0.97      0.95       200
           1       0.64      0.38      0.47        24

    accuracy                           0.91       224
   macro avg       0.79      0.68      0.71       224
weighted avg       0.90      0.91      0.90       224

```

#### Naive Bayes
- **Confusion Matrix**: 
[[182, 18], [1, 23]]
- **Classification Report**:
```
              precision    recall  f1-score   support

           0       0.99      0.91      0.95       200
           1       0.56      0.96      0.71        24

    accuracy                           0.92       224
   macro avg       0.78      0.93      0.83       224
weighted avg       0.95      0.92      0.92       224

```

#### K-Nearest Neighbors
- **Confusion Matrix**: 
[[195, 5], [2, 22]]
- **Classification Report**:
```
              precision    recall  f1-score   support

           0       0.99      0.97      0.98       200
           1       0.81      0.92      0.86        24

    accuracy                           0.97       224
   macro avg       0.90      0.95      0.92       224
weighted avg       0.97      0.97      0.97       224

```

## Conclusion
The choice of model may vary depending on the specific needs of the application. For this dataset:
- **Logistic Regression** performed well with high accuracy and is highly interpretable.
- **Naive Bayes** provided a quick and effective solution with competitive accuracy.
- **K-Nearest Neighbors** showed the highest accuracy but may require more tuning and computational resources.

The final model choice will depend on the importance of accuracy, interpretability, and computational efficiency.

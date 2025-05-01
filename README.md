**Bank Marketing Prediction**

Description:
The project uses the UCI Bank Marketing dataset.
The objective is to predict whether or not a client will subscribe to a term deposit.
This is done by comparing two mdodels, Logistic Regression and Random Forest whilst also focusing more on handling class imbalance and evaluating precision, recall, and F1-Score.

Steps:
- Mapped binary features (yes/no) to 0/1.
- One-hot encoded multiclass categorical columns.
- Scaled numerical columns with MinMaxScaler.
- Split in to train/test sets (80/20).

Models:
Logistic Regression ('class_weight= 'balanced', 'solver='liblinear')
Random Forest ('max_depth=2, class_weight='balanced')

Metrics used:
- Confusion Matrix
- Precision
- Recall
- F1-score


 Sample Results

| Model                | Precision (Class 1) | Recall (Class 1) | F1-Score (Class 1) |
|---------------------|---------------------|------------------|--------------------|
| Logistic Regression | 0.42                | 0.83             | 0.56               |
| Random Forest       | 0.30                | 0.75             | 0.43               |

Logistic Regression performed better.


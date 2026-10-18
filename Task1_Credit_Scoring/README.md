
# Credit Scoring Model

## Project Overview
This project uses machine learning to predict whether a credit card customer may default on future payments. It uses customer financial and repayment information to train and evaluate classification models.

## Dataset
- **Source:** UCI Machine Learning Repository
- **Dataset:** Default of Credit Card Clients
- **Records:** 30,000
- **Input features:** 23
- **Target:** `Y` — 0 = No Default, 1 = Default

## Machine Learning Models
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Balanced Random Forest Classifier

## Evaluation Metrics
Models were evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

## Results

The Balanced Random Forest model achieved:
- **Accuracy:** approximately 80%
- **Default-class precision:** 54%
- **Default-class recall:** 53%
- **Default-class F1-score:** 54%
- **ROC-AUC:** 0.7702

The balanced model improved the detection of defaulting customers compared with the original Random Forest model, although some false positives and false negatives remain.

## Project Files
- `credit_scoring.ipynb` — notebook containing data preparation, model training, and evaluation
- `credit_scoring_model.pkl` — saved Balanced Random Forest model
- `requirements.txt` — required Python libraries
- `README.md` — project documentation

## Technologies Used
Python, Pandas, NumPy, Matplotlib, Scikit-learn, Joblib, and UCI ML Repository tools.

## Disclaimer
This project is for educational purposes only. Its predictions should not be used as the sole basis for real credit or financial decisions.

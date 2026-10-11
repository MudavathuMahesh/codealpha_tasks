# Heart Disease Prediction using Machine Learning

## Project Overview
This project compares machine learning classification algorithms to predict the recorded heart disease outcome from patient data. It was developed as part of the CodeAlpha Machine Learning Internship.

## Objective
To train and evaluate classification models using structured medical data.

## Dataset
- Source: [Heart.csv dataset](https://github.com/reisanar/datasets/blob/master/Heart.csv)
- Records: 303
- Original columns: 15
- Target column: `AHD`
- Target labels: `Yes` and `No`

The `Unnamed: 0` index column was removed. Missing values in `Ca` and `Thal` are handled by the preprocessing pipeline.

## Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Joblib
- Google Colab

## Workflow
1. Load and inspect the dataset.
2. Remove the index column.
3. Separate features and target.
4. Split into training and test sets.
5. Handle missing values.
6. Scale numerical features.
7. Encode categorical features.
8. Train and compare models.
9. Evaluate model performance.
10. Save the selected pipeline.

## Models
- Logistic Regression
- Decision Tree
- Random Forest

## Results

Results on a 61-record test set:

| Model | Accuracy | Precision | Recall | F1-score |
|---|---:|---:|---:|---:|
| Logistic Regression | 90.16% | 86.67% | 92.86% | 89.66% |
| Random Forest | 86.89% | 81.25% | 92.86% | 86.67% |
| Decision Tree | 73.77% | 71.43% | 71.43% | 71.43% |

Logistic Regression achieved the highest F1-score in this experiment.

## How to Run
1. Open `disease_prediction.ipynb` in Google Colab.
2. Run the notebook cells in order.
3. Load the dataset from the linked CSV source.
4. Train and evaluate the models.

## Limitations
- This is an educational machine learning project, not a medical diagnostic tool.
- The dataset is relatively small.
- Results from one train/test split do not establish clinical reliability.
- Further validation on independent data would be required for real-world use.

## Author
Mahesh Mudavathu

Machine Learning Intern — CodeAlpha

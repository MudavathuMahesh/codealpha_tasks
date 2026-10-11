# codealpha_tasks

# Heart Disease Prediction using Machine Learning

## Project Overview
This project uses machine learning classification algorithms to predict the recorded heart disease outcome from patient data. It was developed as part of the CodeAlpha Machine Learning Internship.

## Objective
To train and compare classification models using structured medical data and evaluate their performance on a held-out test set.

## Dataset
- Source: [Heart.csv dataset](https://github.com/reisanar/datasets/blob/master/Heart.csv)
- Number of records: 303
- Original columns: 15
- Target column: `AHD`
- Target labels: `Yes` and `No`

The `Unnamed: 0` index column was removed before training. The dataset contains missing values in `Ca` and `Thal`, which are handled by the preprocessing pipeline.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Joblib
- Google Colab

## Machine Learning Workflow
1. Load and inspect the dataset.
2. Remove the unnecessary index column.
3. Separate features and target.
4. Split the data into training and testing sets.
5. Handle missing values.
6. Scale numerical features.
7. Encode categorical features using one-hot encoding.
8. Train and compare classification models.
9. Evaluate the models using classification metrics.
10. Save the selected model.

## Models Evaluated
- Logistic Regression
- Decision Tree
- Random Forest

## Results

Evaluation on a 61-record test set:

| Model | Accuracy | Precision | Recall | F1-score |
|---|---:|---:|---:|---:|
| Logistic Regression | 90.16% | 86.67% | 92.86% | 89.66% |
| Random Forest | 86.89% | 81.25% | 92.86% | 86.67% |
| Decision Tree | 73.77% | 71.43% | 71.43% | 71.43% |

Logistic Regression achieved the highest F1-score among the three models in this experiment.

## Evaluation
The models were evaluated using accuracy, precision, recall, F1-score and a confusion matrix. The test set contained 61 records, so the results may vary with a different split or dataset.

## How to Run
1. Open `disease_prediction.ipynb` in Google Colab.
2. Run the notebook cells in order.
3. The dataset is loaded from the linked public CSV source.
4. Train and evaluate the models.
5. The selected pipeline can be saved as `disease_prediction_model.pkl`.

Install dependencies using:

`pip install -r requirements.txt`

## Project Files
- `disease_prediction.ipynb` — notebook containing the code and analysis.
- `disease_prediction_model.pkl` — saved Logistic Regression pipeline.
- `requirements.txt` — Python package dependencies.
- `README.md` — project documentation.

## Limitations
- This is an educational machine learning project, not a medical diagnostic tool.
- The dataset is relatively small.
- Results from one train/test split do not establish clinical reliability.
- Further validation on independent data would be required before any real-world use.

## Author
Mahesh Mudavathu

Machine Learning Intern — CodeAlpha

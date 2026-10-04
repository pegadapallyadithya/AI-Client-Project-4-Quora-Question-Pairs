# Quora Question Pairs — Duplicate Question Detection

## Project Overview

This project develops a machine learning model to identify whether two Quora questions have essentially the same meaning.

The project was completed as part of the DataMites AI Client Project 4 — Quora Question Pairs.

## Business Problem

Duplicate or semantically equivalent questions can appear repeatedly on a question-answering platform. Automatically identifying duplicate question pairs can help reduce redundant content and improve question organization.

## Project Objective

Build a classification model that predicts whether a pair of questions is a duplicate.

## Dataset

The project uses the Quora Question Pairs dataset.

Key fields include:

- `question1`
- `question2`
- `is_duplicate`

The original dataset is not included in this repository.

## Approach

1. Loaded and inspected the dataset.
2. Performed data-quality checks.
3. Analyzed the target class distribution.
4. Analyzed question lengths and question-pair characteristics.
5. Prepared the question-pair data.
6. Created stratified train, validation, and test splits.
7. Built a baseline classification model.
8. Performed hyperparameter tuning using GridSearchCV.
9. Selected the final model based on validation performance.
10. Evaluated the final model on the held-out test set.
11. Generated classification metrics and a confusion matrix.
12. Performed error analysis and reviewed example predictions.

## Evaluation

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

## Results

The complete analysis, model development, evaluation results, visualizations, and example predictions are available in the Jupyter Notebook included in this repository.

## Limitations

- Duplicate-question labels can contain ambiguity or noise.
- Some questions may have subtle differences in meaning that are difficult to classify.
- Model performance depends on the quality and coverage of the available labelled data.

## Future Improvements

- Use transformer-based sentence embeddings.
- Explore more advanced NLP architectures.
- Improve semantic feature engineering.
- Evaluate the model on additional unseen question data.

## Project Structure

```text
AI-Client-Project-4-Quora-Question-Pairs/
│
├── AI_Client_Project_4_Quora_Question_Pairs.ipynb
└── README.md

## How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/pegadapallyadithya/AI-Client-Project-4-Quora-Question-Pairs.git
cd AI-Client-Project-4-Quora-Question-Pairs

2. Install Required Libraries
pip install pandas numpy scikit-learn matplotlib seaborn jupyter

3. Prepare the Dataset
Download the Quora Question Pairs dataset and place the required dataset file locally.
The original dataset is not included in this repository.

4. Open the Jupyter Notebook
jupyter notebook

Open:
AI_Client_Project_4_Quora_Question_Pairs.ipynb
5. Run the Notebook
Run the notebook cells sequentially to reproduce the complete analysis and machine learning workflow.
Technology Stack
Technology	Purpose
Python	Core programming language
Pandas	Data loading, cleaning and analysis
NumPy	Numerical operations
Scikit-learn	Machine learning, preprocessing and evaluation
GridSearchCV	Hyperparameter tuning
Matplotlib	Data visualization
Seaborn	Statistical visualization
Jupyter Notebook	Project development and documentation


Machine Learning Workflow
Data Loading → Data Quality Checks → EDA → Feature Preparation → Train/Validation/Test Split → Baseline Model → GridSearchCV → Final Model → Evaluation → Error Analysis
Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

Limitations
- Duplicate-question labels may contain ambiguity or noise.
- Some questions can have subtle differences in meaning.
- Model performance depends on the quality and coverage of the labelled dataset.

Future Improvements
- Use transformer-based sentence embeddings.
- Explore advanced NLP architectures.
- Improve semantic feature engineering.
- Evaluate the model on additional unseen question data.

Author
Pegadapally Adithya
AI / Machine Learning Project

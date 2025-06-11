# CAT1
# Student Exam Performance Prediction

## 📌 Problem Statement
This project aims to predict whether a student will pass or fail based on various demographic and academic features. The dataset used is the "Student Performance Data Set" from the UCI Machine Learning Repository (student-mat.csv).

## 🧠 Approach

1. **Data Preprocessing**
   - Loaded the dataset.
   - Handled categorical features using one-hot encoding.
   - Created a binary target column `pass` (1 if G3 >= 10, else 0).
   - Cleaned and explored the dataset.

2. **Feature Engineering**
   - Selected important features such as `G1`, `G2`, `Medu`, `Fedu`, `studytime`, `internet`, etc.
   - Converted necessary columns to boolean or numerical types.

3. **Train/Test Split**
   - Split data into 80% training and 20% testing using `train_test_split`.

4. **Model Training**
   - Trained two models:
     - Logistic Regression
     - Decision Tree Classifier

5. **Model Evaluation**
   - Used accuracy, F1-score, and confusion matrix.
   - Selected the better model based on these metrics.

## 📊 Results & Interpretation

| Model               | Accuracy | F1 Score | Notes                          |
|--------------------|----------|----------|--------------------------------|
| Logistic Regression| 0.7368   | 0.8415   | Performs well with low false negatives. |
| Decision Tree       | 0.7416   | 0.8412   | Slightly higher accuracy, but similar performance. |

**Best Model:** Decision Tree (based on accuracy, though both models are close).

## 📁 Repository Structure

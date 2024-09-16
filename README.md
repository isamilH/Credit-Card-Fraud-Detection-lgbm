# Credit Card Fraud Detection with Gradient Boosting

This repository contains a notebook that demonstrates the detection of fraudulent transactions using Gradient Boosting techniques on a highly imbalanced dataset.

## Dataset

The dataset used in this project contains transactions made by credit cards in September 2013 by European cardholders. It includes:

- **284,807 transactions** over two days.
- **492 fraudulent transactions**, representing approximately 0.172% of the total dataset.

### Features

- **Time**: Seconds elapsed between each transaction and the first transaction in the dataset.
- **Amount**: The transaction amount, useful for cost-sensitive learning.
- **V1 to V28**: Principal components obtained via PCA transformation (due to confidentiality, the original features are not available).
- **Class**: Response variable where 1 represents a fraudulent transaction and 0 a normal transaction.

## Project Structure

The notebook is organized into the following sections:

1. **Exploratory Data Analysis (EDA)**: Visualization of transaction distributions, fraud occurrence, and correlation analysis.
2. **Data Preprocessing**: Handling missing data, scaling features, and managing the class imbalance through techniques like oversampling or undersampling.
3. **Modeling**: Training a Gradient Boosting model to classify fraudulent transactions. Various evaluation metrics are applied due to the imbalanced nature of the dataset.
4. **Evaluation**: Use of precision-recall curves, confusion matrices, and AUC-PR to assess model performance.

## Results

The model shows promising results when detecting fraud, despite the significant imbalance in the dataset. Key metrics include:

  1. Precision-Recall AUC: More reliable for imbalanced classification than accuracy.
  2. Confusion Matrix: Helps to understand the number of false positives and negatives.

## Future Work
 1. Experiment with other classification algorithms like Random Forest, XGBoost, or Neural Networks.
 2. Apply advanced techniques for handling imbalanced data (e.g., SMOTE, ADASYN).
 3. Deploy the model using an MLOps pipeline for real-time fraud detection.
   

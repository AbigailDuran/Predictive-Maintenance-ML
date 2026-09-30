# Predictive Maintenance Using Machine Learning

This project uses supervised machine learning to predict machine failures using the AI4I 2020 Predictive Maintenance Dataset.

The goal is to compare multiple classification algorithms and evaluate how well they can identify potential equipment failures based on machine operating conditions.

## Project Objective

Unexpected equipment failure can lead to downtime, increased maintenance costs, and reduced productivity.

This project explores how machine learning can be used for predictive maintenance by analyzing operational data and identifying patterns associated with machine failure.

The project focuses on:

- Preparing and exploring the dataset
- Training multiple classification models
- Comparing model performance
- Evaluating predictions using classification metrics, with emphasis on F1 score
- Examining how machine operating conditions relate to equipment failure

## Dataset

This project uses the **AI4I 2020 Predictive Maintenance Dataset** from the UCI Machine Learning Repository.

The dataset contains 10,000 observations representing simulated industrial machine operating conditions.

### Main Input Features

- Product Type
- Air Temperature
- Process Temperature
- Rotational Speed
- Torque
- Tool Wear

The product type variable includes three quality levels:

- **L** — Low quality
- **M** — Medium quality
- **H** — High quality

### Target Variable

The primary target variable is:

- **Machine Failure**

The model is trained to determine whether a machine failure occurred based on the available operating conditions.

Dataset source:

https://archive.ics.uci.edu/dataset/601/ai4i+2020+predictive+maintenance+dataset

## Machine Learning Workflow

The general workflow for this project is:

1. Explore and understand the dataset
2. Clean and preprocess the data
3. Prepare features and target variables
4. Split the data into training and testing sets
5. Train multiple classification models
6. Evaluate model performance
7. Compare the models using classification metrics

## Model Evaluation

Because machine failures make up a relatively small portion of the dataset, model performance is evaluated using metrics that consider class imbalance.

Evaluation metrics may include:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

The **F1 score** is used as an important comparison metric because it balances precision and recall.

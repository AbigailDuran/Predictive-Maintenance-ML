# Dataset

This project uses the **AI4I 2020 Predictive Maintenance Dataset** from the UCI Machine Learning Repository.

The dataset was created for predictive maintenance research and contains simulated industrial machine operating data.

## Dataset Source

UCI Machine Learning Repository:

https://archive.ics.uci.edu/dataset/601/ai4i+2020+predictive+maintenance+dataset

## Dataset Overview

The dataset contains **10,000 observations** and includes operating conditions, product information, tool wear, and machine failure information.

Each row represents a machine operating condition at a given point in time.

## Features

The main input features used in this project include:

- **Type** — Product quality level:
  - `L` = Low quality
  - `M` = Medium quality
  - `H` = High quality

  The `Type` feature represents the quality category of the product being processed by the machine. The dataset is made up of approximately 50% Low-quality products, 30% Medium-quality products, and 20% High-quality products.

  Product type also affects tool wear in the dataset. Each product category contributes a different amount of wear to the machine tool:

  - `L` products contribute **2 minutes** of tool wear
  - `M` products contribute **3 minutes** of tool wear
  - `H` products contribute **5 minutes** of tool wear

  Because product type is related to how quickly the tool wears, it can provide useful information to the machine learning model when predicting machine failure.
- **Air temperature [K]** — Air temperature in Kelvin
- **Process temperature [K]** — Process temperature in Kelvin
- **Rotational speed [rpm]** — Machine rotational speed
- **Torque [Nm]** — Torque applied during operation
- **Tool wear [min]** — Amount of tool wear in minutes

The dataset also includes identification columns such as:

- **UDI** — Unique identifier
- **Product ID** — Product identifier

These identification columns may be excluded from model training because they do not directly represent machine operating conditions.

## Target Variable

The primary target variable for this project is:

- **Machine failure**
  - `0` = No machine failure
  - `1` = Machine failure

The goal of the machine learning models is to predict whether a machine failure occurs based on the available operating features.

## Failure Types

The dataset also includes several specific failure indicators:

- Tool Wear Failure
- Heat Dissipation Failure
- Power Failure
- Overstrain Failure
- Random Failure

These variables provide additional information about the type of failure that occurred.

## Data Usage

The dataset is used for:

1. Exploratory data analysis
2. Data preprocessing
3. Feature selection
4. Training classification models
5. Evaluating model performance
6. Comparing models using metrics such as precision, recall, and F1 score

## Notes

The AI4I 2020 dataset is synthetic, meaning it was generated to resemble realistic industrial machine conditions rather than collected directly from a physical manufacturing system.

This makes it useful for machine learning experimentation while still representing relationships commonly found in predictive maintenance applications.

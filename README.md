# Machine Learning Project

This Python machine learning project analyzes a dataset and performs various data preprocessing and classification tasks. The project focuses on predicting anxiety symptoms based on different features. 

<!-- TABLE OF CONTENTS -->
## Table of Contents

- [Getting Started](#getting-started)
- [Project Description](#project-description)
- [Results](#results)
- [Conclusion](#conclusion)
- [Acknowledgments](#acknowledgments)

## Getting Started

To get started with this project, follow the instructions below.

### Prerequisites

Make sure you have the following libraries installed:

- `numpy`
- `pandas`
- `scikit-learn`
- `imblearn`
- `matplotlib`

### Installation

1. Clone the repository: git clone https://github.com/your-username/your-repository.git
2. Change to the project directory: cd your-repository
3. Install the required dependencies: !pip install 'dependencyName'

## Dataset

The dataset used in this project is sourced from the following URL:
[Thesis Data](https://raw.githubusercontent.com/sheemasiddiqui/Thesis_Data/main/thesis_data.csv)

### Usage
1. Run the Python colab notebook by simply clicking Open In Colab button on the top right of the code
2. The project details performance of data preprocessing, feature selection, and classification tasks.
3. The results will be displayed in the console.

## Project Steps

1. Loading and Exploring the Dataset:
   - The dataset is loaded from the provided URL using Pandas.
   - Basic information about the dataset is displayed, such as the shape and the first few rows.

2. Data Preprocessing:
   - Irrelevant columns that have no relation to the target column are dropped.
   - Columns with missing values are identified and dropped.
   - The "Height" and "Weight" columns are combined to calculate the BMI (Body Mass Index).
   - Column names are renamed for programming simplicity.

3. Feature Selection:
   - Correlation analysis is performed to identify highly correlated features.
   - The "Height" and "Weight" columns, which are highly correlated with BMI, are dropped.

4. Handling Missing Values:
   - Numeric columns with missing values are filled with their mean values.
   - Nominal columns with missing values are filled with their mode values.

5. Data Encoding:
   - One-Hot Encoding is applied to categorical columns to convert them into numeric representations.

6. Data Balancing:
   - The dataset is balanced using the Synthetic Minority Over-sampling Technique (SMOTE) to address class imbalance.

7. Model Training and Selection:
   - Several classification models, including Logistic Regression, Random Forest, K-Nearest Neighbors, Decision Tree, and Support Vector Machine, are evaluated.
   - Grid search and cross-validation are used to find the best hyperparameters for each model.
   - The F1 score is used as the evaluation metric for model selection.

8. Feature Importance:
   - The feature importance of the selected model (Random Forest) is calculated and displayed.
   - A bar plot is generated to visualize the importance of each feature.

9. Model Evaluation:
   - The selected model (Random Forest) is evaluated using classification metrics such as accuracy, precision, recall, and F1 score.
   - A confusion matrix and an ROC curve are plotted to assess the model's performance.

## Results

The project provides insights into the dataset and predicts anxiety symptoms based on the available features. The best performing model is Random Forest Classifier, which achieves a high F1 score.


## Conclusion

This project demonstrates the process of analyzing a dataset, preprocessing the data, selecting relevant features, training different classification models, and evaluating their performance. The final model achieved good results in predicting anxiety symptoms based on the given features.

## Acknowledgments

- This project is based on real-world data and was developed as part of a thesis project.
- Special thanks to the contributors and maintainers of the libraries used in this project.

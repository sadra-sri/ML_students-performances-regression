# Students Performance – Multiple Linear Regression

This project uses the **Students Performance in Exams** dataset from Kaggle to build a
multiple linear regression model that predicts **math score** based on other exam scores.

## Dataset

- **Name:** Students Performance in Exams  
- **Source:** Kaggle  
- **Link:** https://www.kaggle.com/datasets/spscientist/students-performance-in-exams  

> Note: The dataset file (\`StudentsPerformance.csv\`) is **not** included in this repository.  
> Please download it from Kaggle and place it in the same folder as the notebook.

## Project Overview

In this notebook:

- The dataset is loaded and inspected (head, info, describe)
- Features (X) are selected:
  - \`reading score\`
  - \`writing score\`
- Target (y) is selected:
  - \`math score\`
- The data is split into **train** and **test** sets
- A \`LinearRegression\` model (from scikit-learn) is trained
- The model is evaluated using:
  - R² (coefficient of determination)
  - MSE (Mean Squared Error)
  - RMSE (Root Mean Squared Error)
- An **Actual vs Predicted** plot is created for math scores on the test set  
  with the ideal reference line \`y = x\`

## How to Run

1. Clone the repository:

    git clone https://github.com/sadra-sri/ML_students-performances-regression.git
    cd ML_students-performances-regression

2. (Optional) Create and activate a virtual environment.

3. Install dependencies:

    pip install -r requirements.txt

4. Download the dataset from Kaggle and save \`StudentsPerformance.csv\`
   in the project folder (same directory as the notebook).

5. Run the notebook:

    jupyter notebook students_performance_regression.ipynb

## Current Results

On the test set, the current model achieves approximately:

- **R²:** 0.68  
- **RMSE:** 8.8 (on math scores in the range 0–100)

This is a simple baseline multiple linear regression model.

## Possible Improvements

- Add categorical features (e.g. \`gender\`, \`lunch\`, \`test preparation course\`)
- Try regularization methods (Ridge, Lasso)

- Perform more detailed exploratory data analysis and feature engineering

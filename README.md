# NFL Player Success Machine Learning Project

This repository is the code for a larger research project titled *Analyzing the Effectiveness of a Logistic Regression Model to Predict NFL Player Success Based on Early Performances*.

This repository contains a machine learning project that predicts the success of NFL players based on their physical attributes and performance statistics. The code is written in Python and can be found in the `main.ipynb` file.

## Dataset

The datasets used in this project can be found on [Github](https://github.com/nflverse/nfldata/blob/master/DATASETS.md) and contain data on NFL rosters and draft picks. This data is derived from the [*Pro Football Reference*](https://www.pro-football-reference.com).

## Dependencies

To run the code in this project, you will need the following dependencies:
- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

You can install these dependencies using pip:

```
pip install pandas numpy scikit-learn matplotlib
```

## Running the Code

To run the code, clone the repository and open the `main.ipynb` file in Jupyter Notebook. You can then run each cell to load the dataset, preprocess the data, and train the machine learning models.

## Machine Learning Models

This project trains a logistic regression model to predict the success of NFL players uses K-Fold cross validation to evaluate the model.

The model is evaluated using accuracy, precision, recall, and F1 score. The model was adjusted to use the most accurate predictors.

## Results

The results of the project are analyzed in a separate paper and can be found by running all cells in the `main.ipynb` file.
They include the accuracy, precision, recall, and F1 score of the best performing model on the holdout set of data in addition to the results of K-Fold cross validation.

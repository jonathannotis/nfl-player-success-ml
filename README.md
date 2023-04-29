# NFL Player Success Machine Learning Project

This repository is the code for a larger research project titled *Analyzing the Effectiveness of a Logistic Regression Model to Predict NFL Player Success Based on Early Performances*.

This repository contains a machine learning project that predicts the success of NFL players based on basic data from a player's first two career seasons. The code is written in Python and can be found in the `main.ipynb` file.

## Dataset

The datasets used in this project can be found on [Github](https://github.com/nflverse/nfldata/blob/master/DATASETS.md) and contain data on NFL rosters and draft picks. This data is derived from the [*Pro Football Reference*](https://www.pro-football-reference.com). 

### Variables Used

- **`5_years_later`:** The dependent variable used for this project. A binary value stating whether a player is active on a roster five years after being drafted (meaning they surpassed their rookie contract).
- **`pick`:** The overall draft pick at which the player was selected.
- **Side:** Whether a player plays on offense, defense, or special teams. Reffered to in code as `is_offense`, `is_defense`, and `is_special_teams`. The value representation for this set of variables is binary.
- **Category:** A grouping of positions based on the position's role during play. The format for these variables is `category_[]`. The value representation for this set of variables is binary.
- **Position:** The specific role a player takes on a the field. The format for these variables is `position_[]`. The value representation for this set of variables is binary.
- **Team Drafted:** The team that drafter a player. The format for these variables is `drafted_by_[]`. The value representation for this set of variables is binary.
- **Active Team:** The team a player is playing on for each of their first two years in the league. The format for these variables is `on_[]_year_[]`. The value representation for this set of variables is binary.
- **Games:** The number of regular season games played in for each of a player's first two years in the league. The format for these variables is `games_year_[]`.
- **Starts:** The number of regular season games a player is on the starting roster for in their first two years in the league. The format for these variables is `starts_year_[]`.
- **Approximate Value:** Player's Approximate Value, as defined by the the [*Pro Football Reference*](https://www.pro-football-reference.com), for each of their firt two years. The format for these variables is `value_year_[]`.

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

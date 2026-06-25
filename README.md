# Titanic Survival Prediction using KNN

## Project Overview

This project predicts passenger survival on the Titanic dataset using the K-Nearest Neighbors (KNN) machine learning algorithm.

## Dataset

The dataset contains passenger information such as:

* Passenger Class (Pclass)
* Sex
* Age
* Fare
* Embarked Port
* Family Information

Target Variable:

* Survived (0 = No, 1 = Yes)

## Data Preprocessing

* Removed unnecessary columns

  * Cabin
  * PassengerId
  * Name
  * Ticket
* Filled missing Age values using Mean
* Filled missing Fare values using Mean
* Filled missing Embarked values using Mode
* Applied One-Hot Encoding for categorical features
* Applied MinMax Scaling

## Model

* K-Nearest Neighbors (KNN)
* Hyperparameter tuning using GridSearchCV

Best Parameters:

* n_neighbors = 26
* p = 1 (Manhattan Distance)

Cross Validation Accuracy:

* 81.37%

## Technologies Used

* Python
* NumPy
* Pandas
* Scikit-Learn
* Google Colab

## Output

Generated prediction file:

* titanic_knn_submission.csv

# MACHINE-LEARNING
Titanic Survival Prediction Using Machine Learning
Project Overview
The Titanic Survival Prediction project aims to analyze and predict the survival of passengers aboard the infamous Titanic using machine learning techniques. This project leverages historical passenger data, including attributes such as age, gender, class, fare, and family connections, to build a predictive model. The goal is to explore which factors influenced the likelihood of survival during the tragic sinking of the ship on April 15, 1912.

Dataset
The dataset used for this project is sourced from Kaggle and contains two primary CSV files: train.csv and test.csv.

train.csv: This file contains 891 entries with various features related to the passengers, including:

PassengerId: Unique ID for each passenger.
Survived: Survival status (0 = No, 1 = Yes).
Pclass: Ticket class (1st, 2nd, or 3rd).
Name: Passenger name.
Sex: Gender of the passenger.
Age: Age of the passenger.
SibSp: Number of siblings/spouses aboard.
Parch: Number of parents/children aboard.
Ticket: Ticket number.
Fare: Fare paid for the ticket.
Cabin: Cabin number (not used due to many missing values).
Embarked: Port of embarkation (C = Cherbourg; Q = Queenstown; S = Southampton).
test.csv: This file is used for making predictions. It contains similar features as train.csv but does not include the Survived column.

Data Preprocessing
Before training the machine learning model, the data undergoes several preprocessing steps, including:

Handling missing values by imputing the mean age and using mode for categorical features.
Encoding categorical variables (e.g., converting Sex and Embarked into numerical values).
Dropping unnecessary columns such as PassengerId, Name, Ticket, and Cabin to reduce complexity and noise in the data.
Model Training
The project employs a Logistic Regression model to classify whether a passenger survived or not. The dataset is split into training and testing subsets, allowing the model to learn from the training data and be evaluated on unseen test data.

Results and Evaluation
The model's performance is evaluated using several metrics, including:

Accuracy: The proportion of correctly predicted instances out of the total instances.
Confusion Matrix: A visual representation of the true vs. predicted classifications.

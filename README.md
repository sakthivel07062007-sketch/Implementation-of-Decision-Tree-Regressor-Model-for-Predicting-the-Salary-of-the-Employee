# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Data Setup: Load the CSV and split it into Features (X) and Target (Salary).

2. Encoding & Splitting: Convert text to numbers using One-Hot Encoding and split the data into Training (80%) and Testing (20%) sets.

3. Model Training: Fit the Decision Tree Regressor to the training data, allowing it to learn rules for predicting salaries based on input features.

4. ViSual Output: Generate a Tree Diagram that shows the step-by-step logic and decision splits the model used to reach its predictions.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

import pandas as pd
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split
from sklearn.tree import DecisionTreeRegressor, plot_tree
data = pd.read_csv("Salary (1).csv")
X = data.drop("Salary", axis=1)
y = data["Salary"]
X = pd.get_dummies(X, drop_first=True)
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42)
model = DecisionTreeRegressor(random_state=42)
model.fit(X_train, y_train)
plt.figure(figsize=(25,12))
plot_tree(
    model,
    feature_names=X.columns,
    filled=True
)

plt.title("Decision Tree Regressor")
plt.show()

Developed by: SAKTHIVEL K
RegisterNumber:  212225240133
*/
```

## Output:

<img width="1859" height="889" alt="591824067-e5ae94e4-45a6-4cdc-a517-896d54f6f527" src="https://github.com/user-attachments/assets/9794bc07-5071-43bc-825e-a122d55669a0" />

## Result:

Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.

# Implementation-of-Logistic-Regression-Using-Gradient-Descent

## AIM:
To write a program to implement the the Logistic Regression Using Gradient Descent.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Initialize dataset, weights, and bias.

2. Define the sigmoid function.

3. Compute predicted output using current weights.

4. Update weights and bias using gradient descent.

5. Repeat until convergence and display the result.

## Program:
```
/*
Program to implement the the Logistic Regression Using Gradient Descent.
Developed by: VISHNUPRIYA E
RegisterNumber:212225230308

import numpy as np
import matplotlib.pyplot as plt

# Sample data
X = np.array([1, 2, 3, 4, 5])
y = np.array([0, 0, 0, 1, 1])

# Initialize parameters
w = 0
b = 0
learning_rate = 0.1
epochs = 1000

# Sigmoid function
def sigmoid(z):
    return 1 / (1 + np.exp(-z))

# Gradient Descent
for i in range(epochs):
    z = w * X + b
    y_pred = sigmoid(z)
    
    # Derivatives
    dw = (1/len(X)) * np.sum((y_pred - y) * X)
    db = (1/len(X)) * np.sum(y_pred - y)
    
    # Update
    w = w - learning_rate * dw
    b = b - learning_rate * db

# Output
print("Weight:", w)
print("Bias:", b)

# Plot
plt.scatter(X, y, color='red')
x_line = np.linspace(0, 6, 100)
y_line = sigmoid(w * x_line + b)
plt.plot(x_line, y_line)
plt.xlabel("X")
plt.ylabel("Probability")
plt.title("Logistic Regression using Gradient Descent")
plt.show() 
*/
```

## Output:
<img width="905" height="690" alt="Screenshot 2026-04-29 134158" src="https://github.com/user-attachments/assets/59481fbe-1b37-449a-86d0-563004ab8a50" />



## Result:
Thus the program to implement the the Logistic Regression Using Gradient Descent is written and verified using python programming.


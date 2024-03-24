# Linear Regression with one variable using Python

This project is one of my assignments for the Machine Learning course. In this project, there is a lab to implement linear regression with one variable to predict a restaurant franchise's profits using Python.

## 1. Packages
In this lab, we mainly use two packages: [numpy](www.numpy.org) and [matplotlib](http://matplotlib.org). numpy can process data by working with matrices, and matplotlib can visualize data by plotting graphs. We use the `import` command to import these packages.

## 2. Problem Statement
Based on the data of population and corresponding profits of the cities where the chain has restaurants, and the data of population of the candidate cities, the CEO of the restaurant franchise wants to find the candidate city that can give potentially higher profits.

## 3. Dataset
Load the data by using the command `x_train, y_train = np.loadtxt('ex1data1.txt', delimiter = '\t', unpack=True)`, which can get the population data `x_train` and profit data `y_train` synchronously.   

To get familiar with the data of `x_train` and `y_train`, we can use the commands of `type(x_train)`, `x_train[:5]` and `x_train.shape`.  

We can also use a scatter plot to visualize the data from matplotlib to find the relationship between `x_train` and `y_train`.

## 4. Linear regression
$$f_{w, b}(x) = wx + b$$
This is the linear regression function used to find the relationship between `x` (population) and `y` (profit). In this model, we need to find the proper parameter $(w,b)$ for our dataset.  

In order to find the best $(w, b)$ for our dataset, we can use cost function $J(w,b)$ to evaluate it. It means that the best fitting $(w, b)$ has the smallest cost $J(w, b)$.  

To find the smallest possible cost $J(w, b)$, we can use the **gradient descent** method.

## 5. Compute Cost
We build the `compute_cost()` function to compute the cost $J(w, b)$. In this function, we use a loop to get the sum of the costs of every training example. After that, we check our code by running the test code.

## 6. Gradient descent
We build the `compute_gradient` function to compute the total gradient. In this function, we use another loop to get the total gradient for the parameters $w, b$ from all the training examples. After that, we check our code by running the test code.

##
After the above steps, we get the functons of `compute_cost()` and `compute_gradient`. Using these two functions, batch gradient descent and appropriate learning rate, we can obtain the optimal parameters $w, b$.

We can use the final parameters $w, b$ to compute the predictions for all the dataset and plot the linear fit.

Finally, we use the final parameters $w, b$ to predict the profits of the candidate cities, so that the CEO can choose the candidate city that can make the highest profit.


## Related link: 
[C1_W2_Linear_Regression](https://github.com/x24-byte/CPSC5616CS_ML/blob/main/C1_W2_Linear_Regression.ipynb)




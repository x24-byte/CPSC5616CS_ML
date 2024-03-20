# Neural Networks for Handwritten Digit Recognition, Multiclass

This project is one of my second assignment for the Machine Learning course. In this project, there is a practice lab to implement neural networks for handwritten digit recognition in multiclasses.

## 1. Packages
In this lab, we used a lot of packages: numpy, tensorflow, matplotlib, and logging. Numpy can process data by working with matrices, tensorflow can create machine learning models, matplotlib can visualize data by plotting graphs and logging can emit log messages from Python programs. We use the `import` command to import these packages.  

## 2. ReLU Activation
$$a = max(0, z)$$
In this lab, the new activation Rectified Linear Unit (ReLU) is used for countinuous linear relationship. When the input is less than zero, the output is zero, and when the input is not less than zero, the output is linear.  

## 3. Softmax Function
$$a_j = \frac{e^{z_j}}{ \sum_{k=0}^{N-1}{e^{z_k} }} \tag{1}$$
The softmax function is used to convert the output layer's N outputs into decimals that between 0 and 1 that represents probabilities of every outputs.  
The N outputs is a vector $\mathbf{z}$, and $\mathbf{z}$ comes from the linear fuction $z = \mathbf{w} \cdot \mathbf{x} + b$.    

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

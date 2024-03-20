# Neural Networks for Handwritten Digit Recognition, Multiclass

This project is one of my second assignment for the Machine Learning course. In this project, there is a practice lab to implement neural networks for handwritten digit recognition in multiclasses.

## 1. Packages
In this lab, we used a lot of packages: NumPy, Tensorflow, matplotlib, and logging. Numpy can process data by working with matrices, tensorflow can create machine learning models, matplotlib can visualize data by plotting graphs and logging can emit log messages from Python programs. We use the `import` command to import these packages.  

## 2. ReLU Activation
$$a = max(0, z)$$  
In this lab, the new activation Rectified Linear Unit (ReLU) is used for countinuous linear relationship. When the input is less than zero, the output is zero, and when the input is not less than zero, the output is linear.  

## 3. Softmax Function
$$a_j = \frac{e^{z_j}}{\sum_{k=0}^{N-1} e^{z_k}}$$  
The softmax function is used to convert the output layer's N outputs into decimals that between 0 and 1 that represents probabilities of every outputs. The sum of these N decimals is 1.
The N outputs is a vector $\mathbf{z}$, and $\mathbf{z}$ comes from the linear fuction $z = \mathbf{w} \cdot \mathbf{x} + b$.    
We can use NumPy to implement the sofmax function, and tensorflow also has this function.  

## 4. Neural Networks
In this project, we implement a neural network to do multiclass classification which is to figure out ten handwritten numbers from 0 to 9.  
The dataset of this project has 5000 examples of handwritten digits, and each example has 400 digits.  
The model has three layers: two layers using ReLU activations and an output layer using linear activation. Each layer has 25 units, 15 units and 10 units respectively. 
We can use Tensorflow to implement this model's layers, and use softmax fuction to convert outputs to probabilities.  

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

# Practice Lab: Decision Trees

This project is my third assignment for the Machine Learning course. In this project, there is a practice lab to implement a decision tree and apply it to classify whether a mushroom is edible or poisonous.  

## 1. Packages
In this lab, we mainly use two packages: NumPy and matplotlib. Numpy can process data by working with matrices, and matplotlib can visualize data by plotting graphs. We use the `import` command to import these packages.   

## 2. Problem Statement
We are launching a business focused on cultivating and marketing wild mushrooms. To differentiate between safe-to-eat and toxic mushrooms, we aim to classify them by their physical traits. We already have some data that needs to be analyzed to ensure only edible mushrooms are sold.  

## 3. Dataset
There are 10 examples of mushrooms and they have three features: Cap Color (Brown or Red), Stalk Shape (Tapering or Enlarging), and Solitary (Yes or No). And there is one label: Edible (1 indicating yes or 0 indicating poisonous).   

We turned the feature values into 0 or 1 for easy implementation: 
- X_train contains three features for each example: Brown Color (1-"Brown", 0-"Red"), Tapering Shape (1-"Tapering Stalk Shape", 0-"Enlarging"), and Solitary (1-"Yes", 0-"No").
- y_train is whether the mushroom is edible: y = 1 indicates edible, y = 0 indicates poisonous.  

## 4. Decision Tree Refresher
### 4.1 Calculate entropy
The helper function `compute_entropy` computes the entropy at a node. This function takes in a numpy array that indicates whether the examples in that node are edible or poisonous. The entropy is calculated as  
$$H(p_1) = -p_1 \text{log}_2(p_1) - (1- p_1) \text{log}_2(1- p_1)$$
  

##
After the above steps, we can build a neural networks model for recognizing handwritten digits.  


## Related link: 
[C2_W2_Assignment](https://github.com/x24-byte/CPSC5616CS_ML/blob/main/C2_W2_Assignment.ipynb)


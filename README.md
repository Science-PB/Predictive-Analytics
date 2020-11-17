# -Logistic-Regression-algorithm
Image recognition with Logistic Regression algorithm


# Introduction
Linear models are a class of models that are widely used in practice and have been the subject of detailed study over the past few decades, and their history goes back to over a hundred years. Linear models are also widely used in classification problems. Let's look at the binary classification. In this case, the forecast is obtained using the following formula:

<img width="838" alt="Screen Shot 2020-11-17 at 1 55 27 AM" src="https://user-images.githubusercontent.com/66921930/99356550-57d9a500-2878-11eb-9420-bacdf88f2cdb.png">

To get the result, we set the value to exactly zero for the predicted value. If the result is less than zero, then the value is -1, respectively, if the result is greater than 0, then the value is +1.

# Logistic Regression method

Overview: For this project, we will be using Logistic Regression to predict the image. To do
this, we will build 10 different models and use the softmax function to calculate the correct results after calculating the probabilities.

Data: The dataset consists of 784 features columns and 1 target column.(Figure 2). Target refers to numbering from 0 to 9 and applies to different clothes.(Figure 1).

<img width="440" alt="Screen Shot 2020-11-17 at 1 56 53 AM" src="https://user-images.githubusercontent.com/66921930/99356551-58723b80-2878-11eb-9f74-8e23f1d68f70.png">


<img width="974" alt="Screen Shot 2020-11-17 at 1 57 00 AM" src="https://user-images.githubusercontent.com/66921930/99356552-58723b80-2878-11eb-814c-ee6a51ff1749.png">

# Python 3 Code:

1) First, we load all the necessary libraries and functions that we need to develop the algorithm. Further, the columns in the dataset will be named, the training and test dataset will be loaded into the environment.


2) We need to build 10 different models for each of the digits and find the probability of image by pickles. Let's start with 0. To do this, create a zero_label column where the dummy variables will be located. Let's create features and target variables for test and train dataset.


3) Fit logistic regression and calculate the probabilities


4) We get an accuracy: 0.956 which is a very good result. We visualize the digit 0.


5) We repeat the same algorithm for the digit one. create a zero_label column where the dummy variables will be located.


6) Then fit the Logistic Regression for the dataset and compute predicted probabilities.


7) We got an accuracy of 0.991. Let's visualize the result.


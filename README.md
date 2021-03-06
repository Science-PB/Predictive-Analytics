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

<img width="768" alt="Screen Shot 2020-11-17 at 1 59 16 AM" src="https://user-images.githubusercontent.com/66921930/99356827-d898a100-2878-11eb-8fd7-5545b4b738e0.png">


2) We need to build 10 different models for each of the digits and find the probability of image by pickles. Let's start with 0. To do this, create a zero_label column where the dummy variables will be located. Let's create features and target variables for test and train dataset.

<img width="529" alt="Screen Shot 2020-11-17 at 1 59 47 AM" src="https://user-images.githubusercontent.com/66921930/99356832-d9c9ce00-2878-11eb-85d3-d7d157a45020.png">

3) Fit logistic regression and calculate the probabilities

<img width="873" alt="Screen Shot 2020-11-17 at 2 08 33 AM" src="https://user-images.githubusercontent.com/66921930/99357461-f286b380-2879-11eb-936e-9d3dc51e8b5e.png">


4) We get an accuracy: 0.956 which is a very good result. We visualize the digit 0.

<img width="479" alt="Screen Shot 2020-11-17 at 2 08 50 AM" src="https://user-images.githubusercontent.com/66921930/99357462-f31f4a00-2879-11eb-9e5e-c8f7e7013fcc.png">

5) We repeat the same algorithm for the digit one. create a zero_label column where the dummy variables will be located.

<img width="502" alt="Screen Shot 2020-11-17 at 2 09 04 AM" src="https://user-images.githubusercontent.com/66921930/99357464-f3b7e080-2879-11eb-9895-d848928ae9be.png">

6) Then fit the Logistic Regression for the dataset and compute predicted probabilities.

<img width="561" alt="Screen Shot 2020-11-17 at 2 00 45 AM" src="https://user-images.githubusercontent.com/66921930/99356839-db939180-2878-11eb-9429-15288f17d906.png">

7) We got an accuracy of 0.991. Let's visualize the result.

<img width="532" alt="Screen Shot 2020-11-17 at 2 01 00 AM" src="https://user-images.githubusercontent.com/66921930/99356840-dc2c2800-2878-11eb-8de2-68b623580f52.png">


8) We do the same algorithm of actions for the remaining digits.

<img width="286" alt="Screen Shot 2020-11-17 at 2 11 27 AM" src="https://user-images.githubusercontent.com/66921930/99357736-6e80fb80-287a-11eb-9798-10c2db653673.png">
<img width="353" alt="Screen Shot 2020-11-17 at 2 11 36 AM" src="https://user-images.githubusercontent.com/66921930/99357739-6f199200-287a-11eb-8f91-a797dbd003e4.png">
<img width="413" alt="Screen Shot 2020-11-17 at 2 11 42 AM" src="https://user-images.githubusercontent.com/66921930/99357740-6fb22880-287a-11eb-8772-9cb43cca1786.png">
<img width="437" alt="Screen Shot 2020-11-17 at 2 11 47 AM" src="https://user-images.githubusercontent.com/66921930/99357742-704abf00-287a-11eb-8576-3c256e2cd0bc.png">
<img width="416" alt="Screen Shot 2020-11-17 at 2 11 53 AM" src="https://user-images.githubusercontent.com/66921930/99357744-70e35580-287a-11eb-939d-67ed997f9692.png">
<img width="462" alt="Screen Shot 2020-11-17 at 2 11 58 AM" src="https://user-images.githubusercontent.com/66921930/99357746-717bec00-287a-11eb-8379-5a765a818939.png">
<img width="393" alt="Screen Shot 2020-11-17 at 2 12 04 AM" src="https://user-images.githubusercontent.com/66921930/99357748-717bec00-287a-11eb-89d6-416a8cbeef03.png">
<img width="605" alt="Screen Shot 2020-11-17 at 2 12 09 AM" src="https://user-images.githubusercontent.com/66921930/99357749-717bec00-287a-11eb-991a-0aaaa69e2976.png">



9) Next, we create a dataframe with all the obtained probabilities for the clothes.

<img width="897" alt="Screen Shot 2020-11-17 at 2 14 36 AM" src="https://user-images.githubusercontent.com/66921930/99357942-d1729280-287a-11eb-8674-7c539b1c2666.png">


10) We use the softmax function and define the label for the clothes.

<img width="974" alt="Screen Shot 2020-11-17 at 2 15 02 AM" src="https://user-images.githubusercontent.com/66921930/99357947-d2a3bf80-287a-11eb-92dd-2ce5d148e03e.png">

11) We create a confusion matrix to better understand where the model was right and where it made a mistake.

<img width="676" alt="Screen Shot 2020-11-17 at 2 15 26 AM" src="https://user-images.githubusercontent.com/66921930/99357948-d3d4ec80-287a-11eb-909d-aac8ab81db2d.png">






# CSCI480 Spring 2021
# Homework 4
# Due: 11:59pm 03/26/2021

# Q1: Generate an artifical dataset based on the following model(This dataset will used in Q2 and Q3).
~~~~
y = 1 + 2*x1 + 3*x2 
~~~~
+ Note:
  - two features x1 and x2
  - create 500 data points in the dataset
  - do not forget to add noise when calculating y values
  - split it into training set and test set 

# Q2: Design and train a linear regression model using Mini-Batch Gradient Descent.
+ Hint: 
  - you can use the grad_mse() and mse() functions for Batch Gradient Descent directly, but remember you only need to use a mini-batch(part) of the whole training set when updating the paramters.
  - To select a mini batch, you can decide a mini batch size, then randomly select the mini batch from the whole training set in each iteration. You can also use other ideas to select the mini batch.
  - use mse to evaluate the model
# Q3: Design and train a ridge model, or a lasso model, or a ElasticNet model.
+ Note: 
  - You can choose any model for the regularization.
  - You can choose your own hyper-parameters.
  - use mse to evaluate the model
# Q4: Design and train a logistic regression model to predict the digit is an even-number or not-even-number in MNIST dataset.
+ Note: 
  - use 60000 data points as the training set and 10000 as test set.
  - use accuracy to evaluate the model
# Q5: Design and train a softmax regression model to predict the digit is less than 3, between 3 and 6, or greate than 6 in MNIST dataset..
+ Note: 
  - use 60000 data points as the training set and 10000 as test set.
  - use accuracy to evaluate the model

# Step 1: Please complete Q1-Q5
# Step 2: Please save the answers in a Python Jupyter notebook file, name it as "CSCI480_Homework4_JohnDoe(0123456).ipynb", where 0123456 is your BeeCard number, and sumbit it on [Blackboard](https://blackboard.sau.edu/webapps/login/)
+ Note: in the .ipynb file, if you need to provide some comments or explanation for your work, you need to change the type of the file to Markdown. Here is the [basic syntanx for Markdonw](https://www.markdownguide.org/basic-syntax/)

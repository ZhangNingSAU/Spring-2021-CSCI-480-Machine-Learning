# CSCI480 Spring 2021
# Homework 3
# Due: 11:59pm 03/15/2021

# Q1: Downlaod the MNIST dataset and use 60000 instances as the training set, and 10000 as the test set(use all the 70000 instances in the dataset).
# Q2: Design and train a binary classifier to predict even-number or not-even-number.
# Q3: Design and train a multiclass classfier to predict the digit is less than 3, between 3 and 6, or greate than 6.
+ Hint: to create new targets, we have many different ways. for example
~~~~
# method 1
y_true = [0,1,2,3,4,5,6,7,8,9]
for i in range(len(y_true)):
    if y_true[i]<3:
        y_true[i] = 0
    elif y_true[i]>6:
        y_true[i] = 2
    else:
        y_true[i] = 1
        
# method 2
y_true = [0,1,2,3,4,5,6,7,8,9]

def convert_digit(digit):
    if digit<3:
        return 0
    elif digit>6:
        return 2
    else:
        return 1

y_true = [convert_digit(digit) for digit in y_true]

# method 3
y_true = [0,1,2,3,4,5,6,7,8,9]
def convert_digit(digit):
    if digit<3:
        return 0
    elif digit>6:
        return 2
    else:
        return 1
y_true= list(map(convert_digit, y_true))
~~~~
# Q4: Design and train a multilabel classifier to predict two labels: even-number and prime-number.
Hint: to create new target for prime-number, of course you can define a isPrime function(you can find a lot on the internet) then replace the convert_digit function with it. 
Or you can do it in a much simpler way because we only need to deal with 10 digits(only 2,3,5,7 are prime numbers).
~~~~
y_true = [0,1,2,3,4,5,6,7,8,9]
y_true = [digit in [2,3,5,7] for digit in y_true]
~~~~

# Note:
+ Use accuracy as the metric in Q2.
+ Use precision and recall/sensitivity as the metrics in Q3.
+ Use F1-score as the metric in Q4.
+ Use cross validation for one model(you can choose any one).
+ Bonus: Plot the ROC curve and cacluate AUC for the binary classification model in Q2(10 points).
+ Bonus: Error analysis for the multiclass classification model in Q3(10 points).
+ Execute your code before the submission.

# Step 1: Please complete Q1-Q4
# Step 2: Please save the answers in a Python Jupyter notebook file, name it as "CSCI480_Homework3_JohnDoe(0123456).ipynb", where 0123456 is your BeeCard number, and sumbit it on [Blackboard](https://blackboard.sau.edu/webapps/login/)
+ Note: in the .ipynb file, if you need to provide some comments or explanation for your work, you need to change the type of the file to Markdown. Here is the [basic syntanx for Markdonw](https://www.markdownguide.org/basic-syntax/)

# Neural_Network_Charity_Analysis
## Overview of the loan prediction risk analysis
Bek’s come a long way since her first day at that boot camp five years ago—and since earlier this week, when she started learning about neural networks! Now, she is finally ready to put her skills to work to help the foundation predict where to make investments. With my knowledge of machine learning and neural networks, I’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. To do so, I'll do the folowing tasks:
 - Preprocessing Data for a Neural Network Model
 - Compile, Train, and Evaluate the Model
 - Optimize the Model

## Results
### Data Preprocessing
Cleaning the data is a major part of modelling, so I've divided the provided dataset to target and features data. Also I've dropped some of the noisy data. 
 - As a target data, I've chosen the IS_SUCCESSFUL column to check whether the application got approved or not. 
 - In order to know that, I've selected the rest of the columns except the "EIN" and "NAME" columns that were removed from the dataset. 
The following data shows the selected data which includes the target column and the features columns:

  ![image](https://user-images.githubusercontent.com/80184581/130852202-84ba5bc8-5cb9-451d-83da-d593b3341767.png)
  

### Compiling, Training, and Evaluating the Model
As we see in the following code script: 
 - We've chosen two hidden layers for our data with 80 and 50 neurons after a trial and error process to get the highest accuracy rate for the model. 
 - In addition, we used the ReLu activation function for the hidden layers since it is the most used activation function in neural networks due to its simplifying output and the Sigmoid activation function for the output layer to transform the output to a range between 0 and 1. 

  ![image](https://user-images.githubusercontent.com/80184581/130852397-09a94d8f-80c0-4bef-830e-ee845eb5fefa.png)

 - Our target model performance was 75%, but our model performance was a little bit less than that. 
 - However, we haven't stopped from optimizing the model to reach the target. I've:
  - Dropped the USE_CASE column from the data
  - Increased the neurons in each hidden layer
  - Added a third hidden layer
  - Changed the activation function of the output layer from Sigmoid to ReLu

## Summary
In general, although the results are not as expected, this model has absolutely helped us to predict where to make investments. Other models may show better results like the Random Forest or Support vector machine models since the amount of code required to build and train these models is notably less than the comparable deep learning model. As a result, many data scientists will prefer to use them by default, then turn to deep learning models, as needed. 

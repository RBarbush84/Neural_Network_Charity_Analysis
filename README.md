# Neural_Network_Charity_Analysis
## Overview
### Purpose
The purpose of this analysis is to build a neural network model to predict how Alphabet Soup can make the most impactful positive donations to different organizations, and determine which organizations Alphabet Soup helps fund will be the most beneficial to donate to.

## Results
### Data Preprocessing
- The IS_SUCCESSFUL variable was the target of this model, to determine if donations made by Alphabet Soup were successful.
- The variables that were features to try to predict if donations are successful were APPLICATION_TYPE, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS and ASK_AMT.
- The EIN and NAME variables were neither targets nor features of the model and were dropped from the input data.

### Compiling, Training and Evaluating the Model
- The first model used 2 hidden layers, the first had 80 neurons and the second had 30 neurons. The 2 hidden layers used ReLU function, and the output layer used the sigmoid function. The accuracy for this model was 72.90%.

#### Original Model Code
![Original Model Code](https://github.com/RBarbush84/Neural_Network_Charity_Analysis/blob/main/Resources/Original%20Model%20Code.png)

#### Original Model Results
![Original Model Results](https://github.com/RBarbush84/Neural_Network_Charity_Analysis/blob/main/Resources/Original%20Model%20Results.png)


- This model was not able to achieve 75% target performance. It only reached 72.90% accuracy, so some further steps were taken to attempt to improve the performance of the model.

- The below steps were taken to try to increase model performance to the 75% accuracy target.
  - Attempt 1- Adding neurons to the second hidden layer

I changed the amount of neurons in the second hidden layer from 30 to 60 in an attempt to increase model performance. This led to an accuracy of 72.86% for the model, and did not increase performance to the target.

#### Optimization Attempt 1 Code
![Opt 1 Code](https://github.com/RBarbush84/Neural_Network_Charity_Analysis/blob/main/Resources/Opt%201%20Code.png)

#### Optimization Attempt 1 Results
![Opt 1 Results](https://github.com/RBarbush84/Neural_Network_Charity_Analysis/blob/main/Resources/Opt%201%20Results.png)

  - Attempt 2- Adding a third hidden layer to the model

For this attempt, I added a third hidden layer to the model that had 30 neurons. This resulted in an accuracy of 72.77% for the model, which does not increase the model's performance to the target.

#### Optimization Attempt 2 Code
![Opt 2 Code](https://github.com/RBarbush84/Neural_Network_Charity_Analysis/blob/main/Resources/Opt%202%20Code.png)

#### Optimization Attempt 2 Results
![Opt 2 Results](https://github.com/RBarbush84/Neural_Network_Charity_Analysis/blob/main/Resources/Opt%202%20Results.png)

  - Attempt 3- Using a Leaky ReLU activation function for the hidden layers

On the third attempt to increase model performance, I changed the activation function used in the hidden layers from ReLU to Leaky ReLU. This change to the model resulted in an accuracy score of 72.90%, and did not increase performance to the 75% target.

#### Optimization Attempt 3 Code
![Opt 3 Code](https://github.com/RBarbush84/Neural_Network_Charity_Analysis/blob/main/Resources/Opt%203%20Code.png)

#### Optimization Attempt 3 Results
![Opt 3 Results](https://github.com/RBarbush84/Neural_Network_Charity_Analysis/blob/main/Resources/Opt%203%20Results.png)

## Summary
Neither the original model nor any of the subsequent attempts at optimizing the model were able to reach the target accuracy score of 75%. The original model had an accuracy score of 72.90%, but none of the attempts to optimize the model were able to improve upon that accuracy.

Some other possible recommendations to try to optimize the model and reach the target accuracy score could include re-bucketing some of the feature variables, such as the ASK_AMT variable or further increasing the number of hidden layers or the number of neurons used in those hidden layers. The accuracy did not appear to vary too much as fitting the model was reaching the end of the process, so it does not look like increasing the number of epochs would help increase accuracy and optimize the model.

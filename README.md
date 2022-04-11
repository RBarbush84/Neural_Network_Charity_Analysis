# Neural_Network_Charity_Analysis
## Overview
### Purpose
The purpose of this analysis is to build a neural network model to predict how Alphabet Soup can make the most impactful positive donations to different organizations, and which organizations Alphabet Soup helps fund will be the most beneficial to donate to.

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


- able to achieve 75% target performance
- steps to try to increase model performance

## Summary
summarize results and provide recommendation (how a different model could help solve the problem)

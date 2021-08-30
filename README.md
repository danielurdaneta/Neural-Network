# Neural Network

## Overview of the analysis

The purpose of this project was to create a Deep Learning Model that can predict whether applicants will be successful if funded by Alphabet Soup. We did this using Python, Pandas, TensorFlow and Scikit-Learn.

## Results

### Data Preprocessing
 
- What variable(s) are considered the target(s) for your model?

The target variable is column "IS_SUCCESSFUL" whose values classify whether a company used the money effectively or not

- What variable(s) are considered to be the features for your model?

Our features variables are the following:

APPLICATION_TYPE — Alphabet Soup application type <br>
AFFILIATION — Affiliated sector of industry <br>
CLASSIFICATION — Government organization classification <br>
USE_CASE — Use case for funding <br>
ORGANIZATION — Organization type <br>
STATUS — Active status <br>
INCOME_AMT — Income classification <br>
SPECIAL_CONSIDERATIONS — Special consideration for application <br>
ASK_AMT — Funding amount requested <br>

- What variable(s) are neither targets nor features, and should be removed from the input data?

First, we just removed the EIN and NAME variables because they are just identification columns with no significant value for our model, as we will see later, we also removed another column trying to optimize our model.

### Compiling, Training, and Evaluating the Model

- How many neurons, layers, and activation functions did you select for your neural network model, and why?

We selected 3 hidden layers, the first one with 80 neurons and the other two with 30 neurons each, we used "Relu" activation function for the hidden layers and "Sigmoid" for the output layer. After training our model with more than 3 hidden layers and 80 neurons, we determined that there is no significant improvement in the model's predictions, and the training time increased considerably, in the other hand, we tried different activation functions like "tanh" and "softsign" but Relu yield the best results.

- Were you able to achieve the target model performance?

After several attempts, we were able to have a model with an accuracy in our training data set of 74.46%, slightly below our target performance of 75%.

- What steps did you take to try and increase model performance?

We determine that removing the "SPECIAL_CONSIDERATIONS" column yield slightly better results, we tried different activation functions but Relu yield the best results, we increased the number of hidden layers from 2 to 3 and had better results, and we increased the number of epochs from 100 to 2000 with similar results.

## Summary

We can say that our model's performance of 72% is not bad, but taking in consideration that a bad prediction may result in millions of dollars in lost, we recommend to create a Random Forest model which may yield better results.



# Neural Network

## Overview of the analysis

The purpose of this project was to create a Deep Learning Model that can predict whether applicants will be successful if funded by Alphabet Soup. We did this using Python, Pandas, TensorFlow and Scikit-Learn.

## Results

### Data Preprocessing
 
- What variable(s) are considered the target(s) for your model?

The target variable is column "IS_SUCCESSFUL" whose values classify whether a company used the money effectively or not

- What variable(s) are considered to be the features for your model?

Our features variables are the following:

APPLICATION_TYPE — Alphabet Soup application type
AFFILIATION — Affiliated sector of industry
CLASSIFICATION — Government organization classification
USE_CASE — Use case for funding
ORGANIZATION — Organization type
STATUS — Active status
INCOME_AMT — Income classification
SPECIAL_CONSIDERATIONS — Special consideration for application
ASK_AMT — Funding amount requested

- What variable(s) are neither targets nor features, and should be removed from the input data?

First, we just removed the EIN and NAME variables because they are just identification columns with no significant value for our model, as we will see later, we also removed another column trying to optimize our model.


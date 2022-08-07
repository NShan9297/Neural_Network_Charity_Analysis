# Neural_Network_Charity_Analysis

# Overview
A non-profit foundation, Alphabet Soup,  was looking to optimize their funding by making sure the organizations that they donate to would make change, or make a "successful"impact.The main goal of this project was to assist with creating a binary classifier that will be able to predict success of organizations to know who to donate to and what orgs are too risky.

# Results

## Target Variables(s)
The target variable is "IS_SUCCESSFUL", we are looking to see if the orgs used monies donated to make an impact or not

## Variable(s) Considered to be Features
Variables considered to be features are all those columns that were not dropped:
Application type, affiliation, classification, use case, organization, income amount, special considerations, and ask amount

## Variables neither target or Features
EIN, NAME, STATUS(all are active)

## How many neurons, layers, and activation functions were selected and why?
for all models, I used 2 hidden layers, the number of neurons was kept the same for one model(110) and the others had more or less.The bin sizes were also increased in one of my models. 

Hidden layers were kept the same as a means of trying to test what other factors, smaller or larger, impacted the model. 
Neurons were adjusted in an effort to increase the performance--we did not see overfitting 
Bin sizes were increased simply to explore the effect they had on the model

## Target model performance achieved?
the target model was not achieved, the highest accuracy was 69-70%% or so, with the initial model and with decreasing

## Steps taken to try to increase model performance
1st was making bins larger, with all initial parameters the same we see a decrease in the accuracy rate from the original model
2nd was adding more neurons, accuracy decreased but not by much--from 69.76 to 69.5%
3rd was changing just the activation function which dramatically decreased the accuracy of the model-from 69.5% to 44%, this is likely due to input and hidden layers not changing
4th (for further testing)- here, to see if a working theory I had in mind (dropping more columns that are not as useful would increase the accurcay of the model.). Here I also dropped the Status column as all were considered to be "Active" or 1. Here the accuracy was 69.1%. 

# Summary
Overall, I would say that the sigmoid function is the best activation function, at least between tanh and sigmoid, to use for this model. The number of neurons alone will not improve accuracy, I believe the a more refined number of neurons, paired with dropping more columns, would yield the highest accuracy for this model. 

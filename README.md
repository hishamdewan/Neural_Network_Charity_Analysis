# Neural Network Charity Analysis
The purpose of this analysis is to use machine learning and neural networks to create a binary classifier that is capable of predicting whether charity applicants will be successful if funded by Alphabet Soup. Alphabet Soup is an organization that is trying to determine which charities could be successful and should be provided funds.

### Resources

- Data sources: [charity_data.csv](https://github.com/hishamdewan/Neural_Network_Charity_Analysis/blob/main/Resources/charity_data.csv) 
- Tools used: Python, Pandas, scikit-learn, tensorflow, Google Colab

## Results 

As part of the analysis, the following questions are answered:

### Data Preprocessing

- What variable(s) are considered the target(s) for your model?

The target for column for the model is "IS_SUCCESSFUL", which indicates whether the money was used effectively.

- What variable(s) are considered to be the features for your model?

The following variables are features used as input for training and testing the model: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL CONSIDERATIONS, ASK_AMT.

- What variable(s) are neither targets nor features, and should be removed from the input data?

The following variables are neither targets nor features and were removed: EIN, NAME.

### Compiling, Training, and Evaluating the Model

- How many neurons, layers, and activation functions did you select for your neural network model, and why? 
 
The neural network model has two input layers and an output layer. The model uses Relu Acitivation function as it is good at dealing with complex dataset with numerous features and efficient with time. Additional information on the model provided below:

![summary_model](/Resources/summary_model.png)

- Were you able to achieve the target model performance?

The target performance of the model was 75% but the model fell just short and achieved an accuracy score of 72.6%.

![target_model_performance](/Resources/target_model_performance.png)

- What steps did you take to try and increase model performance?

I created an auto optimizer function to calculate the best combination of layers, neurons, and activation function to improve model accuracy. The optimization only marginally improved the performance of the model: the optimized model achieved an accuracy score of 72.8%.

![updated_model_performance](/Resources/updated_model_performance.png)

## Summary 

- The neural network model achieved an accuracy score of 72.6% and fell just short of the 75% target. The automatic optimized model achieved an accuracy score of 72.8%. 
- The model could be tested with additional epochs, neurons, and layers to see if the auto optimizer function produces better results.


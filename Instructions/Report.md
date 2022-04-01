### Report on Neural Network Model

# Overview
## The purpose of this analysis was to assess the performance of the deep learning model I created for AlphabetSoup

# Results
## Data Preprocessing
* The target for our model is IS_SUCCESSFUL
* The variables that are the features for our model are: 
1. AFFILIATION
2. CLASSIFICATION
3. USE_CASE
4. ORGANIZATION
5. STATUS
6. INCOME_AMT
7. SPECIAL_CONSIDERATIONS
8. ASK_AMT

* The variables that are neither targets nor features, and should therefore be removed from the input data, are:
1. EIN
2. NAME

## Compiling, Training, and Evaluating the Model
* In the final version of my neural network model, I selected 6 hidden layers, each with 8 neurons, and a sigmoid activation functions. I kept adding layers and nodes because the prior model settings did not seem to be improving.
* Even with that number of layers and nodes, I was not able to achieve the target model performance of 75%
* On the first attempt, I used 2 hidden layers with 5 nodes and the relu activation function. I used the sigmoid activation function on the output layer and 5 epocs. In the next version of the model I added a hidden layer, incrased the number of nodes to 10 each, and left the number of epocs at 5. In my third effort, I used 6 hidden layers with 8 nodes each, leavine the activation functions alone, and increased the number of epochs to 50. Finally, in my 4th and final try, I simply change the scalar from the standard scalar to the minmax scalar, because I thought the Ask Amount may be affecting the performance of the model. My approach to all of these changes was to make single, incremental changes to the settings of the model to try to isolate the setting that was holding back the performance.   

# Summary
## Here I will summarize the overall results of the deep learning model. 
* In summary, I used the features in the provided dataset to try to create a binary classifier that is capable of predicting 
whether applicants will be successful if funded by Alphabet Soup.
* I think with more time and resources a model could be found to solve this classification problem.

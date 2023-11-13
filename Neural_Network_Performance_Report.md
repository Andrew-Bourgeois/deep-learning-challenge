# **Module 21 - deep-learning-challenge - Report**

# Alphabet Soup Funding Outcome Neural Network

## **Overview of the Analysis**

The purpose of this analysis was to create and train a neural network which would be able to accurately predict, within a reasonable degree of accuracy, whether an applicant for funding with the Alphabet Soup company will be a successful venture.

In order to accomplish this goal and train our neural network, Alphabet Soup provided a CSV file with over 34k applicants who they have funded, along with metadata data about those companies and whether the venture resulted in success.

Using machine learning and neural network design we created our initial model using two hidden layers, with 6 and 4 neurons respectively and an output layer using the 'sigmoid' activation.

We made three additional attempts to optimize the model and increase the accuracy by changing such parameters as the numbe of neurons in the layes and changing the number of layers. The target accuracy was at or over 75%.

## **Results**

### **Data Preprocessing**
* What variable(s) are the target(s) for your model?
    *   The target feature for our model was the 'IS_SUCCESSFUL' feature.
* What variable(s) are the features for your model?
    * The featuers we chose to use for teachign our model were, ['APPLICATION_TYPE', 'AFFILIATION','CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS']
* What variable(s) should be removed from the input because they are neither targets nor features.
    * We dropped both the 'EIN' and 'NAME' features as they were merely identification metadata about the companies.

### **Compiling, Training, and Evaluating the Model
* How many neurons, layers, and activation functions did you select for your neural network model and why?
    * We started with two hidden layers using the 'relu' activation, and an out put layer using the 'sigmoid' activation.
    * We used 6 heurons for the first hidden layer and 5 for the second in order to: first, limit the amount of time it would take to run our first set of 100 epochs, and second, the  hope we would be able to have a good starting accuracy with which to further design our optimzations from.
* Were you able to achieve the target model performance?
    * We were not able to reach the desired target performance of 75% accuracy.
* What steps did you take to increase model performance?
    * See model/optimization info below:

### **Initial model:**
The initial model resulted in a loss of 0.5594 and accuracy of 0.7251.

### **OPTIMIZATION ATTEMPT #1** - add more neurons to the hidden layers. Increase the 1st hidden layer to 20 and the second to 10.

* RESULT - Although it took longer to run the results were similar, between 72% and 73%. In fact, the accuracy was slightly worse

### **OPTIMIZATION ATTEMPT #2** - increase the number of hidden layers and reduce the number of neurons in the second and third hidden layers.

* RESULT - Again, the model failed to obtain the desired 75% accuracy. The model continued to struggle to get even to a 73% accuracy.

### **OPTIMIZATION ATTEMPT #3** - For a final optimization attempt we will further increase the count threshold of the 'Other' bins for both the 'APPLICATION_TYPE' and 'CLASSIFICATION' features. We will set the 'APPLICATION_TYPE' to 1000, and 'CLASSIFICATION' to 2000.

* RESULT - We again failed to even get to 73% accuracy with our optimized model.

## **Summary**

Overall we were able to consistently train and test a neural network which can accurrately predict the success outcome of a funding venture 72.5% of the time. It would fall upon the risk tolerance of the Alphabet Soup company to decide if this 72.5% accuracy is close enough to the target 75% for them to move forward with implementing the model in their decision making process.

In the future I would change the model to try a different input activation and increase the number of nodes and hidden layers. Often the shape of the input data can be an important factor in the accuracy and success of a model. While increasing the number of hidden layers and neurons in each layer can improve the overall accuracy as well.


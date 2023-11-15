# deep-learning-challenge
UNC-CH-DA Module 21 Challenge - Deep Learning and Neural Networks
* Andrew Bourgeois

## **INSTRUCTIONS**

* To run the code clone the repository to your local machine
* Navigate to the /deep-learning-challenge/Deep_Learning_Challenge/ folder: Here you will find the AlphabetSoupCharity.ipynb, AlphabetSoupCharity_Optimization.ipynb, their corresponding .h5 files per the instrucitons, and the Neural_Network_Performance_Report.md.
* The Python notebooks were written using Colab, so you will see a button at the top of each will open the notebooks online in Colab. Alternatively you can open them locally, just esnure you have the proper libararies/packages avaialble to import, and update any output paths.
* NOTE: To be able to output the files to your own Google Colab be sure to:
    * mount your own google drive by running the first block of code
    * update the output paths to the proper folders in your Google drive.

## **BACKGROUND**

A nonprofit foundation named Alphabet Soup would like a tool which can help it select which of their funding applicants are most likely to be a successful venture. We were tasked to use our knowledge of machine learning and neural networks, use the provided historical dataset and develop a binary classifier to predict whether an applicant venture is likely to be successful or not if funded by Alphabet Soup.

Alphabet Soups business team provided a CSV of more than 34,000 historical funding ventures includeing a number columns including company metadata and their success outcomes:

* EIN and NAME—Identification columns
* APPLICATION_TYPE—Alphabet Soup application type
* AFFILIATION—Affiliated sector of industry
* CLASSIFICATION—Government organization classification
* USE_CASE—Use case for funding
* ORGANIZATION—Organization type
* STATUS—Active status
* INCOME_AMT—Income classification
* SPECIAL_CONSIDERATIONS—Special considerations for application
* ASK_AMT—Funding amount requested
* IS_SUCCESSFUL—Was the money used effectively


## **REQUIREMENTS**

## **Preprocess the Data (30 points)**

* Create a dataframe containing the charity_data.csv data , and identify the target and feature variables in the dataset (2 points)

* Drop the EIN and NAME columns (2 points)

* Determine the number of unique values in each column (2 points)

* For columns with more than 10 unique values, determine the number of data points for each unique value (4 points)

* Create a new value called Other that contains rare categorical variables (5 points)

* Create a feature array, X, and a target array, y by using the preprocessed data (5 points)

* Split the preprocessed data into training and testing datasets (5 points)

* Scale the data by using a StandardScaler that has been fitted to the training data (5 points)

## **Compile, Train and Evaluate the Model (20 points)**

* Create a neural network model with a defined number of input features and nodes for each layer (4 points)

* Create hidden layers and an output layer with appropriate activation functions (4 points)

* Check the structure of the model (2 points)

* Compile and train the model (4 points)

* Evaluate the model using the test data to determine the loss and accuracy (4 points)

* Export your results to an HDF5 file named AlphabetSoupCharity.h5 (2 points)

## **Optimize the Model (20 points)**

* Repeat the preprocessing steps in a new Jupyter notebook (4 points)

* Create a new neural network model, implementing at least 3 model optimization methods (15 points)

* Save and export your results to an HDF5 file named AlphabetSoupCharity_Optimization.h5 (1 point)

## **Write a Report on the Neural Network Model (30 points)**

* Write an analysis that includes a title and multiple sections, labeled with headers and subheaders (4 points)

* Format images in the report so that they display correction (2)

* Explain the purpose of the analysis (4)

* Answer all 6 questions in the results section (10)

* Summarize the overall results of your model (4)

* Describe how you could use a different model to solve the same problem, and explain why you would use that model (6)

## **RESOURCES**

* The provided starter code and the class examples from the UNC-CH-DA Module 21.

* In order to complete the callback to save the model's weights every 5 epochs: https://stackoverflow.com/questions/51186330/save-model-weights-at-the-end-of-every-n-epochs 
# Neural_Network_Charity_Analysis

## Overview of the analysis

  We are finally ready to put our skills to work to help the foundation predict where to make investments. From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization. With our knowledge of machine learning and neural networks, we will use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. For this project, we will create a neural network by using Data Manipulation, creating training and testing sets, and finally analyzing the models created.
  
## Results

### Data Processing

- The variable we are considering as the target in our model is the "IS_SUCCESSFUL" column.
- The variables we are considering to be features are the "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT",             "SPECIAL_CONSIDERATIONS" and "ASK_AMT" columns. 
- The variables that are neither targets nor features and should be removed are the "EIN" and "NAME" columns. 

### Compiling, Training, and Evaluating the Model

#### Attempt 1

- 2 Hidden Layers.
- 80 neurons (Layer1), 30 neurons(Layer2).
- Used Relu and Sigmoid Activations Functions since sigmoid is best for binary classifcation problems as this and relu is for nonlinear datasets.

![](https://github.com/Mousse10/Neural_Network_Charity_Analysis/blob/main/Resources/Capture1.PNG)

#### Attempt 2

- 2 Hidden Layers.
- 80 neurons (Layer1), 30 neurons(Layer2).
- Used Relu and Sigmoid Activations Functions since sigmoid is best for binary classifcation problems as this and relu is for nonlinear datasets.
  Removed "USE_CASE_Other","AFFILIATION_Other" columns.

![](https://github.com/Mousse10/Neural_Network_Charity_Analysis/blob/main/Resources/Capture2.PNG)

#### Attempt 3

- 3 Hidden Layers
- 80 neurons (Layer1), 30 neurons(Layer2), 15 neurons(Layer3).
- Used Relu and Sigmoid Activations Functions since sigmoid is best for binary classifcation problems as this and relu is for nonlinear datasets.
- Removed "USE_CASE_Other","AFFILIATION_Other" columns.

![](https://github.com/Mousse10/Neural_Network_Charity_Analysis/blob/main/Resources/Capture3.PNG)

#### Attempt 4 

- 3 Hidden Layers
- 80 neurons (Layer1), 30 neurons(Layer2), 15 neurons (Layer3).
- Reordered Relu and Sigmoid Activations
- Used the original dataset

![](https://github.com/Mousse10/Neural_Network_Charity_Analysis/blob/main/Resources/Capture4.PNG)

  Following our attempts, we came close but were not able to achieve the target model performance. We tried removing noisey variables, adding neurons, adding hiden layers and we tried changing the ctivation function of hidden layers or output layers. 

## Summary

  The deep learning neural network model did not reach the target of 75% accuracy. Considering that this target level is pretty average we could say that the model is not outperforming. Since we are in a binary classification situation, we could use a supervised machine learning model such as the Random Forest Classifier to combine a multitude of decision trees to generate a classified output and evaluate its performance against our deep learning model.



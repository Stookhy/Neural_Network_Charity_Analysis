# Neural_Network_Charity_Analysis

## Overview of the analysis

  1.  Compare the differences between the traditional machine learning classification and regression models and the neural network models.
  2.  Describe the perceptron model and its components.
  3.  Implement neural network models using TensorFlow.
  4.  Explain how different neural network structures change algorithm performance.
  5.  Preprocess and construct datasets for neural network models.
  6.  Compare the differences between neural network models and deep neural networks.
  7.  Implement deep neural network models using TensorFlow.
  8.  Save trained TensorFlow models for later use.

## Results

  ### Data Preprocessing
   ### What variable(s) are considered the target(s) for your model?
   
   *  The target variables in the model is checking to see if the target is marked as successful in the DataFrame, which indicates that Alphabet has successfully funded this initiative.
    
   #### What variable(s) are considered to be the features for your model?
   
   *  The IS_SUCCESSFUL is the feature column targeted for this dataset.
   *  The model will predict whether the non-profit will be successful based on the independent columns in the data set.
    
   #### What variable(s) are neither targets nor features, and should be removed from the input data?
   
   *  The NAME and EIN columns should be removed from the input data. They provide no impact on the target variables.
   *  Therefore, they do not increase the model accuracy and removing them will increase the overall efficiency of the code.
  
  ### Compiling, Training, and Evaluating the Model
   #### How many neurons, layers, and activation functions did you select for your neural network model, and why?
    
   Were you able to achieve the target model performance?
    
   What steps did you take to try and increase model performance?

## Summary

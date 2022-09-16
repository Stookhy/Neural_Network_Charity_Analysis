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
   
   ![This is an image](https://github.com/Stookhy/Neural_Network_Charity_Analysis/blob/main/Resources/Model.png?raw=true)
   
   ![This is an image](https://github.com/Stookhy/Neural_Network_Charity_Analysis/blob/main/Resources/Optimize%20the%20Model.png?raw=true)
  
  ### Compiling, Training, and Evaluating the Model
   #### How many neurons, layers, and activation functions did you select for your neural network model, and why?
   
   *  In the optimized model, layer 1 started with 120 neurons and a relu activation. For layer 2, it dropped to 80 neurons and continued with the relu activation. 
   *  From there, the sigmoid activation is the better fit for layers 3 (40 neurons) and layer 4 (20 neurons).
    
   #### Were you able to achieve the target model performance?
   
   *  No. The target for the model was 75%, but the model could only produce was 72.7% maximum accuracy.
    
   #### What steps did you take to try and increase model performance?
   
   *  To increase model performance, all columns were reviewed. In addition, the SPECIAL_CONSIDERATIONS and STATUS were dropped, which increased the number of neurons and layers. Other activations were tried such as tanh, but the range that model produced went from 40% to 68% accuracy. 
   *  The linear activation produced the worst accuracy, around 28%. The relu activation at the early layers and sigmoid activation at the latter layers gave the best results.

![This is an image](https://github.com/Stookhy/Neural_Network_Charity_Analysis/blob/main/Resources/Alphabet%20Soup%20Charity%20.png?raw=true)

![This is an image](https://github.com/Stookhy/Neural_Network_Charity_Analysis/blob/main/Resources/Alphabet%20Soup%20Optimization.png?raw=true)

## Summary

   The sigmoid and relu activations provide a 72.7% accuracy, which is the best outcome that the model could produce. A recommendation is to try the random forest classifier, given that this variable is less impacted by outliers.

   Feedback: run it on epoch = 50

   The deep learning model predicted approximately 73.03% of the data correctly, which is less than the 75% target. For Alphabet Soup’s, the percentage would need to be higher to meet its purpose.

   To conclude, the deep learning model is a good start to generate accurate predictions. However, to help Alphabet Soup, we would need to tweak the model to allow for further improvements that will generate more accurate results.
   
![This is an image](https://github.com/Stookhy/Neural_Network_Charity_Analysis/blob/main/Resources/Fit%20Model%201.png?raw=true)

![This is an image](https://github.com/Stookhy/Neural_Network_Charity_Analysis/blob/main/Resources/Fit%20Model%202.png?raw=true)

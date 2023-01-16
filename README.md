# Neural Network Charity Analysis
## Overview
The purpose of this analysis is to predict whether applicants will be successful if they received funding. To accomplish this, we implemented neural networks using the TensorFlow platform in Python and created a binary classifier.  

## Results
**Data Preprocessing** 
- The target variable for our model is the 'Is_Successful' column. 
- The following are feature variables for our model: Application Type, Affiliation, Classification, Use Case, Organization, Status, Income Amount, Special Considerations, and Ask Amount. 
- Columns 'EIN' and 'Name' are neither targets nor features and should be removed from the input data. 

**Compiling, Training, and Evaluating the Model**
- The model initially had an accuracy of 72.3% so we tried to optimize it by making 3 different attempts shown below to increase the predictive accuracy. While attempt number 1 and 2 increased the accuracy, attempt number 3 decreased it when we changed the activation of the hidden layer. In the end, we were not able to achieve the target model performance of 75%. 

| Final code with 3 attempts | 
| ------------- | 
| ![Final code](https://user-images.githubusercontent.com/111667387/212580218-621ea700-2506-4fd9-b841-e0c77249b7da.jpg)| 
| **Attempt #1: Added a third hidden layer**
|![1st ](https://user-images.githubusercontent.com/111667387/212580387-d7ac2b7d-c475-4e03-8f26-fcd9f35b123a.jpg)| 
| **Attempt #2: Increased the number of neurons in hidden layers**
|![2nd](https://user-images.githubusercontent.com/111667387/212580410-e2cbe8b5-9941-40db-98b4-9c0789743ffa.jpg)| 
| **Attempt #3: Changed activation function to LeakyReLu**
|![3rd ](https://user-images.githubusercontent.com/111667387/212580452-9eedbf18-e420-4a40-84ed-5892b43027a3.jpg)| 

## Summary 
This deep learning model performed moderately with the highest accuracy of 72.5%. While this does not meet the target performance of 75%, it comes very close and has the potential to surpass it with more changes made. A random forest model can be used to solve this classification problem as they handle categorical features well and can reduce overfitting. 

# Neural_Network_Charity_Analysis
## Overview
In this challenge a nonprofit foundation, Alphabet Soup, is looking for an analysis that will predict which organizations are worth donating to based on their risk. This deep learning neural network evalutes all types of input data and producxes a clear decision making result using the TensorFlow Library. As a part of the challenge we were to explore at least three different neural networks to try and get the accuracy of the model to 75% or more. 

##Results
**Data Preprocessing**
*What variable(s) are considered the target(s) for your model?*
IS_SUCCESSFUL column

*What variable(s) are considered to be the features for your model?*
APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, & ASK_AMT columns

*What variable(s) are neither targets nor features, and should be removed from the input data?*
EIN, NAME, STATUS, & SPECIAL_CONSIDERATION

Code Used for Preprocessing
<img width="638" alt="pp1" src="https://user-images.githubusercontent.com/94129215/165367365-cbb12987-4b5a-4557-be0f-30464b862e01.PNG">
<img width="623" alt="pp2" src="https://user-images.githubusercontent.com/94129215/165367374-04847f8d-47e2-46d1-8123-f3b36b26790b.PNG">
<img width="603" alt="pp3" src="https://user-images.githubusercontent.com/94129215/165367384-494a3766-2e1d-4fdd-bb01-719725845bf4.PNG">


**Compiling, Training, and Evaluating the Model**
*How many neurons, layers, and activation functions did you select for your neural network model, and why?*
* I selected 120 neurons with the activation function of sigmoid for my first layer. My second hidden layer had 50 neurons with a ReLu activation function and my third hidden layer had 18 neurons with a Relu activation function. I decided to change the activation function for the first layer to see if varied activations increased the accuracy, it did not; The accuracy was 35%. Therefore, my next two models only used one activation function for the input.
* My second model I used three hidden layers with 80, 30, and 10 neurons. The activation function was ReLu for all three. The accuracy went up significantly with a 72.8%. I decided to leave the neurons the same and change the activation for all three input values to TanH to see if this would increase the accuracy even further.
* My third model had three hidden layres with 80, 30 and 10 neurons with the activation function TanH for all three. The accuracy percentage stayed relatively the same as the previous model, 72.5% accuracy. 

*Were you able to achieve the target model performance?*
None of my models met the target model performance. 

*What steps did you take to try and increase model performance?*
I first made all the activation functions the same to see if this affected the accuracy percentage, which it did. The next step I took was to change the activation function I used. Using the same activation function for all three inputs had a strong impact on the accuracy, but the change in the activation function had an insignificant impact. 

## Summary
I removed unnecessary data and adjusted neurons as well as activation functions, but was unable to meet the 75% accuracy target. My second model had the highest accuracy percentage with a 72.8%. A Random Forest Model would be my recommendation for a better model. This model would randomly sample the preprocessed data and build several smaller, simplier decision trees. The benefit of this model is that it can be used to rank the value of the input variables increasing its ability to have a higher accuracy percentage for measuring risk. 

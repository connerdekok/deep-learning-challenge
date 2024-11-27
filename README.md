# deep-learning-challenge

Title- Homework Module 21 Alphabet Soup Deep Learning Challenge- Conner Dekok
We looked at a csv for a non profit looking to see who would have the highest success on their ventures. 
Collaboration with other students- I worked with Hunter Becker on this project.  We worked together on completing this project and comparing our results with one another to help make sure we were on the right track when it came to completing this assignment. 
I reviewed the in-class meetings and reviewed the examples we went through in these class lessons. This helped me create some of my starter code along with comments that I used throughout my code. 
I used Microsoft copilot to help correct or ask any questions and bugs I had when creating my code. 


# Overview

* The main purpose of this project was to to try and predict if a charity was succussful or not using a neural network method. 

* We were given a variety of information such as, 'EIN','NAME','APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS','ASK_AMT', 'IS_SUCCESSFUL'. The 'IS_SUCCESSFUL' and column is what we are looking to predict.

# Results 

* What variable(s) are the target(s) for your model?
    * 'IS_SUCCESSFUL' is the only target variable we used.

* What variable(s) are the features for your model?
    * 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS','ASK_AMT'

* What variable(s) should be removed from the input data because they are neither targets nor features?
    *'EIN','NAME'

Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?
    * I had used 2 hidden layers, with using the ReLU activation function in both hidden layers.  The first has a total of 80 neurons and the second had 30. The ouput layer had one sigmoid neuron. 

    * There was two hidden layers of 80 and 30 neurons respecitvely. This allows us to make sure the data still is complex while not being obnoxious. 

    * ReLU is a good activation function to use as it allows the vanishing gradient issues. Sigmoid helps get a full answer of either 1 or 0.  

* What steps did you take in your attempts to increase model performance?

    * When using the Tanh activation function it helps pass through values that include negative values while Relu excludes all negative values.  With Tanh it was an accuracy 72.82%.

![Capture](https://github.com/user-attachments/assets/68ae96d3-f62b-491b-a8e8-428560666143)


    * When adding a third layer and then going back into Relu.
     After underfitting the model with two layers it came out to an accuracy of 72.83%.

![capture 2](https://github.com/user-attachments/assets/5de1dc90-cd22-461b-9aa3-a09cbe8969fc)

    * Then with using less hidden layer neurons it came out with an accuracy of 72.93%.


![Capture3](https://github.com/user-attachments/assets/07ddb89f-e719-420e-aadc-2f3fe9857bcc)


# Summary
All in all we weren't able to find an optimal method to train the model.  The goal we wanted to achieve for accuracy was 75%, but were only 72.83%.  A logistical regression model would be an great reccomendation.  This would be one of the most simply models, but can easily predict whether a charity is succesful or not. 















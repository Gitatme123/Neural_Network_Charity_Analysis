# Neural_Network_Charity_Analysis
The purpose of this analysis is to predict where her foundation should make investments based on data collected from previous donations and the start-ups success after the fact. Beks is looking to build a machine learning model that will accurately predict whether or not to invest in the specific foundation based on historical performances. We will make a binary classifier that will predict whether or not the charities will be successful after funding is given. Beks has 34,000 examples of previous charities that were granted funding and will use this data to train the model.

## Results

### Data Preprocessing
What variable(s) are considered the target(s) for your model?
> The variable considered our target is y, or IS_SUCCESSFUL
> <img width="649" alt="Screen Shot 2022-05-08 at 12 35 59 PM" src="https://user-images.githubusercontent.com/95602006/167308431-6ff98dd1-9bbc-4dea-950e-a5e23f5a6aa3.png">

What variable(s) are considered to be the features for your model?
> X is our varible that contains the many other varibles that are our features for the model. I dropped a few that were unimportant and included the rest below.
> Application Type, Affiliation, Classification, Use Case, Organization, Status, Income Amount, Special Consideration, and Ask Amount 

What variable(s) are neither targets nor features, and should be removed from the input data?
> The EIN and Name, which are essentially just identifying features connecting the data to unique entities. (The identification columns)


### Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
> I chose 3 layers and just 2 different activation functions because i noticed my accuracy did not performan any better when I increased those or changed the activation function.

Were you able to achieve the target model performance?
> Yes I was! But the model never saved it as the best accuracy performance which i thought was strange. I included a screenshot of the accuracy score to show that it did break above .75 at one point!
> <img width="869" alt="Screen Shot 2022-05-08 at 12 28 33 PM" src="https://user-images.githubusercontent.com/95602006/167308593-a9f1c504-e583-4d27-9927-2d5fd47c421d.png">

What steps did you take to try and increase model performance?
> I used a method that creates a new Sequential model with hyperparameter options in an attempt to optimize the model. I also attemped to save the model after 5 epochs in order to train a new model. 


## Summary
The overal results include one score that did break above 75% accuracy. That was included in the screenshot on one of the questions above. 
I think that a logistical regression model might be better because it is a model that mathematically determines its probability of belonging to one of two groups. That is perfect for us because we just need to predict if the funding will be successful or unsuccessful. I think that would be easier considering a neural net is so complex that I can't even explain it that well. The logistical method would be easier to comprehend and explain when we need to tell someone why we believe or do not believe it'll be a good investment to pick x or Y startup.

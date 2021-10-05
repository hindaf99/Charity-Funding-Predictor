# Charity Funding Predictor 

## Overview
This project tried to predict whether applicants will be successful if funded by the Alphabet Soup Co. Alphabet Soup Co wants to provide funding to companies but it needs to know in advance whether it will be successful or not. Money is on the line here and we would not want for it to go to waste.

For this I will create a neural network by using Data Manipulation, creating training and testing sets, and finally analyzing my models that I have created.

## Results
   ### Data Processing
  
   - Target Variable: IS_SUCCESSFUL
   - Feature Variables: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
   - To clean the data I removed the EIN and NAME columns since they have no value to the model.
 
   ### Compiling, Training, and Evaluating the Model Attempt #1
 
   - 2 Hidden Layers
   - 83 neurons (Layer1), 26 neurons(Layer2)
   - I Used Relu and Sigmoid Activations Functions since sigmoid is best for binary classifcation problems as this and relu is for nonlinear datasets.
		 

   ![image](https://user-images.githubusercontent.com/83431185/135941372-0c00e0f6-8881-48fb-9d56-0dc46d49717f.png)

The model's predictive accuracy was under 72%, which means I was not able to achieve the target model performance.
	  
   ### In order to increase the model performance, I considered the following steps: 
   
   - I removed 'STATUS' and 'ASK_AMT' columns
   - I added a third hidden layer with 10 neurons and I chose Relu as activation function 
   - I changed the number of neurons( 80 for layer 1 and 30 for layer 2)
	  
	   
The model's accuracy recording:

  ![image](https://user-images.githubusercontent.com/83431185/135941296-c1d48deb-a2c7-403c-93ba-054685c23efa.png)

	  
## Summary 

in summary my models kept around 72% accuracy score which is decent considering it was an improvement. My recommendation to improve this model would be to find better features to help explain what determines "IS_SUCCESFUL" such as more indepth knowledge of the other associates/ firms being funded. At the end of the day, knowledge is power and if we had more indepth data between all these applications, we can create a better model.


![image](https://user-images.githubusercontent.com/83431185/135945037-e7dd484f-87d2-458e-8d75-d1b50dc14884.png)



![image](https://user-images.githubusercontent.com/83431185/135945127-5d418f6d-f4de-43e5-9c01-dbbc4d4238fe.png)






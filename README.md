Daniel Mlinga   STAT 315

Introduction:
Data – CreditRisk (Stat2Data) 

Researchers conducted a survey of 450 undergraduates in large introductory courses at either Mississippi State University or the University of Mississippi. There were close to 150 questions on the survey, but only four of these variables are included in this dataset. The primary interest for the researchers was factors relating to whether or not a student has ever overdrawn a checking account.
Variables that might be related to whether students overdraw a checking account are:

Age	Age of the student (in years)
Sex	0=male or 1=female
DaysDrink	Number of days drinking alcohol (in past 30 days)
Overdrawn	Has student overdrawn a checking account? 0=no or 1=yes

In this Dataset we are going to build 3 models to predict if the student has Overdrawn their checking account. The predicting variables are Age, Sex, and DaysDrink.


(b).   

Model 1
	
	Summary Statistics 

	 



Residual vs Fitted Plot

	 

	

Q-Q Residuals Plot

	 

	





Empirical Logit Plot

	 


Model 2
	Summary Statistics
	
	 
	Residual vs Fitted Plot

	 

	
Q-Q Residual 	

 

	




Empirical Logit
	
	  

Model 3
	Summary Statistics

 




	Residual vs Fitted Plot
	
		 
	
Q-Q Residual
		
		 






Empirical Logit

		 

(c). 
	Model 1

Overdrawn =  -2.21469+ ( 0.04691* DaysDrink) 

Model 2

Overdrawn =  -5.73866 + ( 0.19321 * Age) 

Model 3

Overdrawn = -2.4092 + ( 0.8558 * Sex)


(d). Besides of all the models having a p-value less than 0.05, suggesting that they are statistically significant in predicting Overdrawn, mod2 (Overdrawn ~ Age) seems to be the best model among the three based on the AIC values. Comparing the AIC values, a lower AIC indicates a better model fit. In this case, mod2 (Overdrawn ~ Age) has the lowest AIC value (334.85), suggesting that it provides the best trade-off between goodness of fit and model complexity. 

(e). Odds Ratio for Age is 1.213141. As "Age" increases by one unit, the odds the student    checking account being Overdrawn is multiplied by approximately 1.21.
 The 95% confidence interval for the odds ratio is calculated to be approximately 1.010536 - 1.456368. This interval provides a range of values within which we can be 95% confident that the true odds ratio lies. In this case, the interval does not include 1, suggesting that the odds ratio for "Age" is statistically significant.

(f) The logistic regression model assumes a linear relationship between the log-odds of the outcome and the predictor variables, the coefficient for "Age" is 0.19321. The significance of this coefficient suggests that as "Age" increases, the log-odds of being "Overdrawn" increases by 0.19321 units. The residual plot shows a downward sloping, suggesting that the relationship may not be adequately captured by a simple linear model. The significance of the coefficients suggests that there is evidence of a relationship between "Age" and the log-odds of being "Overdrawn. “The residual deviance is 330.85 on 436 degrees of freedom, indicating how well the model fits the data. A lower deviance suggests a better fit. The AIC is 334.85, which is a measure of the model's goodness of fit. Lower AIC values indicate better -fitting models.



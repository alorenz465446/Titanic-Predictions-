# Titanic Predictions
![image](https://user-images.githubusercontent.com/107652317/215613872-356354ff-9983-4caf-bb0d-6b8948fbb3a3.png)


## Overview
The sinking of the Titanic is one of the most infamous shipwrecks in history.

On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew.

It took about $7.5 million to build the Titanic and it sunk under the ocean due to collision.

While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

In this challenge, we ask you to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (ie name, age, gender, socio-economic class, etc).

## The Data 

The data has been split into two groups:

training set (train.csv)
test set (test.csv)
The training set should be used to build your machine learning models. For the training set, we provide the outcome (also known as the “ground truth”) for each passenger. Your model will be based on “features” like passengers’ gender and class. You can also use feature engineering to create new features.

The test set should be used to see how well your model performs on unseen data. For the test set, we do not provide the ground truth for each passenger. It is your job to predict these outcomes. For each passenger in the test set, use the model you trained to predict whether or not they survived the sinking of the Titanic.

We also include gender_submission.csv, a set of predictions that assume all and only female passengers survive, as an example of what a submission file should look like.

Data Dictionary

Variable	Definition	          Key
survival	Survival	            0 = No, 1 = Yes
pclass	  Ticket class	        1 = 1st, 2 = 2nd, 3 = 3rd
sex	      Sex	
Age	      Age in years	
sibsp   	# of siblings / spouses aboard the Titanic	
parch   	# of parents / children aboard the Titanic	
ticket	  Ticket number	
fare	    Passenger fare	
cabin	    Cabin number	
embarked	Port of Embarkation	  C = Cherbourg, Q = Queenstown, S = Southampton


Variable Notes

*pclass:* A proxy for socio-economic status (SES)
1st = Upper
2nd = Middle
3rd = Lower

*age:* Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5

*sibsp:* The dataset defines family relations in this way...
Sibling = brother, sister, stepbrother, stepsister
Spouse = husband, wife (mistresses and fiancés were ignored)

*parch:* The dataset defines family relations in this way...
Parent = mother, father
Child = daughter, son, stepdaughter, stepson
Some children travelled only with a nanny, therefore parch=0 for them.


## Contents:

Part1: Exploratory Data Analysis(EDA):
1)Analysis of the features.

2)Finding any relations or trends considering multiple features.

Part2: Feature Engineering and Data Cleaning:
1)Adding any few features.

2)Removing redundant features.

3)Converting features into suitable form for modeling.

Part3: Predictive Modeling
1)Running Basic Algorithms.

2)Cross Validation.

3)Ensembling.

4)Important Features Extraction.


## How Many Survivors 
![image](https://user-images.githubusercontent.com/107652317/215355064-1162743a-92a0-41a4-a817-aae0db507549.png) </br>
![image](https://user-images.githubusercontent.com/107652317/215355077-de394723-6f31-4779-b251-b19468c43bfd.png) </br>
Clearly not many passengers survived the sinking.

Roughly 342 out of 891 passengers survived (38.4%).

To get a better insight on the survival rate different features of the dataset were used. Including sex, port of embarcation, age, and more. 

### Types Of Features
Categorical Features:
A categorical variable is one that has two or more categories and each value in that feature can be categorised by them.For example, gender is a categorical variable having two categories (male and female). Now we cannot sort or give any ordering to such variables. They are also known as Nominal Variables.

Categorical Features in the dataset: Sex,Embarked.

Ordinal Features:
An ordinal variable is similar to categorical values, but the difference between them is that we can have relative ordering or sorting between the values. For eg: If we have a feature like Height with values Tall, Medium, Short, then Height is a ordinal variable. Here we can have a relative sort in the variable.

Ordinal Features in the dataset: PClass

Continous Feature:
A feature is said to be continous if it can take values between any two points or between the minimum or maximum values in the features column.

Continous Features in the dataset: Age


## Results


## Summary


### Resources 
* https://www.kaggle.com/competitions/titanic/overview
* https://www.kaggle.com/competitions/titanic/data

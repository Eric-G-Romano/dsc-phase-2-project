# Multiple Linear Regression Model for King County

![awesome](https://www.racialequityalliance.org/wp-content/uploads/2016/10/assessors_social-1.jpg)

## Introduction 

For this project, we're given real estate data from King County. Our job is to create and solve a business problem using a linear regression model. We have total freedom in who our stakeholders are, and what the business problem is. For this project, I'll be using CRoss-Industry Standard Process for Data Mining (CRISP-DM) as our Data Science Process.

## Business Understanding

As discussed with my group, our project will cater to first time home buyers, generally in their 20's and 30's and perhaps thinking of starting a family. Our regression model will help inform home buyers on which features most impact the overall price, so they can be more strategic when buying their first home. Our hope is to showcase what features may add additional costs, so buyers can reflect whether each feature is worth it or not.  

## Data Understanding 

Our original dataset contains real estate info for houses in 2014-2015, with features including square footage of lot and living, number of bedrooms and bathrooms, grade and condition, whether it's in the waterfront or not, just to name a few. 

Given that we are catering to first time home buyers, we've also added features not included in the dataset, including distance to points of interest, such as transportation centers, medical centers and police stations, criminality rate, school ratings and walking score. 

![alt text](https://github.com/Eric-G-Romano/dsc-phase-2-project/blob/christian_branch/df_hist.png?raw=true)

A histogram of our DataFrame shows which features follow a normal distribution, and it also gives us a great idea of which features we'd need to deal with as categorical. This knowledge will help us later when we process the data using log transformations and dummy variables. 

Upon initial visualizations, we find the following features to have a strong linear relationship with price: square foootage (living, above) and building grade. 


![alt text](https://github.com/Eric-G-Romano/dsc-phase-2-project/blob/christian_branch/img1.png?raw=true)
![alt text](https://github.com/Eric-G-Romano/dsc-phase-2-project/blob/christian_branch/img2.png?raw=true)
![alt text](https://github.com/Eric-G-Romano/dsc-phase-2-project/blob/christian_branch/grade.png?raw=true)

Our added features seem to work out great as well. From the initial look, school rating seems to play a major role in pricing as well. 

![alt text](https://github.com/Eric-G-Romano/dsc-phase-2-project/blob/christian_branch/grade_rank.png?raw=true)




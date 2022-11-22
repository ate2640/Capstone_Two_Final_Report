# Capstone_Two_Final_Report
Submission for Assignment 20.4
# Using Data Science to Predict Delayed Flights

There are fewer things that captivate the human spirit better than flight; there are also fewer things that bring more dread than flight delays. As an avid traveler who's
covered 55 countries, I wanted to take an in-depth look into the factors responsible for one of traveling's greatest trepidations. With a series of Machine 
Learning models and importance features investigations, I uncovered what factors are most common whenever flight delays take place.
The nature of this problem requires for us to view this question as a classification problem, i.e. 'Yes' or 1 for delayed flights, and 'No' or 0 for on-time flights.
As such, I will implement a series of classification metrics in this project.

![image](https://user-images.githubusercontent.com/19559713/203209666-0322b75c-8686-414f-8836-82aa1db8b629.png)

## The Dataset

In addition to the proper classification of delayed and on-time flights, I also want to find the KPIs, i.e. the columns that are most closely associated with delayed
flights. I chose a dataset from Kaggle with 1,200,000+ flights with more than 50 categories over a 15-year span. It provided an abundance of information to successfully
execute the project; it is available [here](https://data.mendeley.com/datasets/j3z5bm7496/1).

## Data Wrangling

Given the size of this dataset, it required a tedious amount of cleaning. With an original size of 61 columns, it contained only 56 after the Wrangling stage (8
deletions as well as 3 columns I created myself). I also removed NaN values by replacing them with the mean of their respective columns. Per the FFA and for the sake 
of this project, I defined a the flights such that any flight with a combined departure and arrival time of more than 15 minutes; conversely, any flight with a combined
departure and arrival delay of up 15 minutes is considered on-time. The Data Wrangling is available [here](https://github.com/ate2640/Capstone_Two_Final_Report/blob/main/Capstone%20Project%20Data%20Wrangling%20by%20Allen%20Edge.ipynb).
![image](https://user-images.githubusercontent.com/19559713/203213195-a10f6166-7e16-4a46-95d4-1b23040cfab5.png)

## Exploratory Data Analysis
I used EDA to better understand the existing relationships among the features of this dataset and to find any trends. I implemented a series of visuals to comprehend my
data, which can be found [here](https://github.com/ate2640/Capstone_Two_Final_Report/blob/main/Capstone%20Project%20Exploratory%20Data%20Analysis%20by%20Allen%20Edge.ipynb).

## Pre-Processing
As the last step before the Machine Learning, it's essential for the data to be ready for fitting. I separated my data into their respective training and test sets,
and the step-by-step is available [here](https://github.com/ate2640/Capstone_Two_Final_Report/blob/main/Capstone%20Project%20Pre-Processing%20and%20Training%20by%20Allen%20Edge.ipynb).

## Modeling
As this is a classification, i.e. a Yes/No problem, I implemented a series of classification metrics, namely a Decision Tree, Logistic Regression and Random Forest.
I also included accompanying Confusion Matrices to better visualize how successfully the tests classified the results from their respective Machine Learning Models.
It is available [here](https://github.com/ate2640/Capstone_Two_Final_Report/blob/main/Flight_Capstone_Modeling_Final.ipynb).

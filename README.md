# Predicting Round Outcomes in Tom Clancy's Rainbow Six Siege

What machine learning model can best predict the outcome of a round in the first-person shooter, Tom Clancy's Rainbow Six Siege?


## Motivation

Tom Clancy's Rainbow Six Siege is one of my favorite video games of all time. I started playing when it first released in 2015 and have continued to play since. The aim of this project 
is to build a machine learning model using R to predict the outcome of a round from the video game Tom Clancy’s Rainbow Six Siege. Tom Clancy’s Rainbow Six Siege is a competitive, 
tactical first-person shooter in which two teams play against each other in objective-based game modes. Each team consists of five players who choose operators with unique 
abilities and both teams take turns defending and attacking an objective. This project will be trying several different machine learning algorithms to find the best performing model on 
this binary classification problem.


## Method and results

After pre-processing the data and performing exploratory data analysis, I decided to fit a total of seven models to the training data. I fit a regular logistic regression, an elastic net 
logistic regression, a k-nearest neighbors model, a random forest, and three types of support vector machines. Using cross validation, I chose the 
random forest model as the model to evaluate using testing data.

Through various iterations of models and the testing of them, I was able to find that the best predictive model for classifying the outcome of a round was a random forest model. It did a decent job at predicting new observations, with a classification accuracy of 0.79 and area under the receiver operating curve of 0.75.


## Repository overview


data

├--   tuning

│    └──   * several rds files to store hyper parameter tuning results

├--   r6_codebook.txt  # explanation of variables contained in data set

├--   rainbow_data.csv  # csv file with relevant data

└──   rainbow_data1.csv  # csv file with relevant data

images

└──   * several png/jpg files

results

├--   final_project.Rmd  # rmd file containing all code for the models and report

├--   final_project.html  # knitted html file

└──   fp.pdf  # pdf version of html

.gitignore

README.md

final_project.Rproj


## More resources

* Link to the Kaggle data set can be found [here](https://www.kaggle.com/datasets/maxcobra/rainbow-six-siege-s5-ranked-dataset).
* StatQuest with Josh Starmer was a great resource for understanding the intuition behind a lot of machine learning models. A link to the YouTube channel can be found [here](https://www.youtube.com/@statquest).


## About

I am the sole contributor to this repository. This project was part of the PSTAT 131: Introduction to Statistical Machine Learning course at UC Santa Barbara.

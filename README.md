# Recipe Rating Classification Project

## Overview
This project aims to classify recipes based on their ratings using various machine learning techniques. The project is carried out in association with IIT Madras.

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Project Structure](#project-structure)
4. [Data Preprocessing](#data-preprocessing)
5. [Model Training](#model-training)
6. [Evaluation](#evaluation)
7. [Results](#results)
8. [Conclusion](#conclusion)
9. [Future Work](#future-work)
10. [Acknowledgements](#acknowledgements)

## Introduction
 This project aims to classify recipes based on their ratings using a dataset from Kaggle. Accurate classification of recipe ratings can help users find the best recipes quickly, improving their cooking experience. Submissions are evaluated on accuracy Score.
 
 ![image](https://github.com/nandanigupta4/Recipe-Rating-Prediction-IITM/assets/82882909/72c2cc58-7495-4f33-bb85-55a74d6a7721)




## Dataset
The dataset contains 10,000+ recipes with features capturing a unique culinary story with details such as recipe names, user reviews, and various key features. 
The dataset is composed of the following files:
train.csv: The training set, which includes the target variable 'rating' and accompanying feature attributes.
test.csv: The test set, containing similar feature attributes but without the target variable 'rating' , as it is the variable to be predicted.
sample_submission.csv: A sample submission file provided in the correct format for competition submissions.

### Columns Description
RecipeNumber: Placement of the recipe on the top 100 recipes list
RecipeCode: Unique ID of the recipe used by the site
RecipeName: Name of the recipe the comment was posted on
CommentID: Unique ID of the comment
UserID: Unique ID of the user who left the comment
UserName: Name of the user
UserReputation: Internal score of the site, roughly quantifying the past behavior of the user
CreationTimestamp: Time at which the comment was posted as a Unix timestamp
ReplyCount: Number of replies to the comment
ThumbsUpCount: Number of up-votes the comment has received
ThumbsDownCount: Number of down-votes the comment has received
Rating: The score on a 1 to 5 scale that the user gave to the recipe. A score of 0 means that no score was given (Target Variable)
BestScore: Score of the comment, likely used by the site to help determine the order comments appear in
Recipe_Review: Text content of the comment

## Exploratory Data Analysis
![image](https://github.com/nandanigupta4/Recipe-Rating-Prediction-IITM/assets/82882909/b221ebfc-4b99-4e51-bbbc-3f52aade6332)





## Data Preprocessing
Data preprocessing involved handling missing values, encoding categorical variables, and normalizing numerical features.
![image](https://github.com/nandanigupta4/Recipe-Rating-Prediction-IITM/assets/82882909/9f98644d-bfa4-49ca-a6e6-af11e61d7393)

![image](https://github.com/nandanigupta4/Recipe-Rating-Prediction-IITM/assets/82882909/7d8ae75b-46a3-483e-a6f3-45e9cc43e9be)





## Model Training
We used several models including logistic regression, random forest, and neural networks. Hyperparameter tuning was performed using GridSearchCV.
![image](https://github.com/nandanigupta4/Recipe-Rating-Prediction-IITM/assets/82882909/62593e0b-7c7e-41c4-84ad-0c41c13da433)





## Evaluation
Models were evaluated using accuracy, precision, recall, and F1-score.
![image](https://github.com/nandanigupta4/Recipe-Rating-Prediction-IITM/assets/82882909/e0d553d2-cf00-49d4-855d-4a3760a00c6d)


![image](https://github.com/nandanigupta4/Recipe-Rating-Prediction-IITM/assets/82882909/e7b5311a-785a-4b92-8ce0-9be9af654694)


![image](https://github.com/nandanigupta4/Recipe-Rating-Prediction-IITM/assets/82882909/e250c6c2-7b55-4339-a8f0-9907ee7a3e70)




## Results
The Stacking classifier achieved the highest accuracy of 78.8 on test data with a ranking of 54 out of 950 participants in kaggle.
![image](https://github.com/nandanigupta4/Recipe-Rating-Prediction-IITM/assets/82882909/ebfbce80-a39e-497f-9dec-360930a75a79)




## Conclusion
The project successfully classified recipes based on ratings with reasonable accuracy. This can significantly aid users in selecting top-rated recipes.

## Future Work
Future work could involve exploring more advanced models and incorporating user reviews to enhance classification accuracy.

## Acknowledgements
Special thanks to IIT Madras for providing this opportunity.



# Predicting the Success Rate of the Upcoming Mobile Application using the Google Playstore Dataset

This GitHub repository contains the code and documentation for the project "Predicting the Success Rate of the Upcoming Mobile Application using the Google Playstore Dataset." The project aims to develop a machine learning model that can predict the rating of a mobile application based on input features. The success of an app is typically measured by user reviews, number of installs, and ratings.

## Problem Definition
The mobile application development industry has become highly competitive, and app developers need to forecast their app's success to ensure they are on the right track. In this project, we investigate the different features of mobile applications and their contribution to the overall success of the application.

## Prior Work
While the mobile application development industry has been extensively studied, this project focuses on predicting the success rate of upcoming mobile applications. Previous research papers have primarily focused on data analysis of existing datasets. This project aims to provide insights into the future impact of mobile applications on the market.

## Dataset Requirement
The project utilizes the Google Playstore dataset, which consists of two datasets: `googleplaystore.csv` and `googleplaystore_user_review.csv`. The `googleplaystore.csv` dataset contains attributes such as `appName`, `category`, `reviews`, `size`, `Installs`, `Type`, `Price`, `contentRating`, `Genres`, `LastUpdated`, and `CurrentVersion`. The target variable for prediction is the `Rating`, and the independent variables are a subset of these attributes. The `googleplaystore_user_review.csv` dataset includes `appName`, `userReview`, and `sentiment` for analyzing the text and predicting the rating.

## Data Cleaning
To understand the dataset's structure, we created a data dictionary. Missing values were handled by either discarding the rows or imputing them with mode values based on the proportion of nulls in each feature. Certain columns, such as `Installs`, `Size`, and `Price`, were converted to numeric types for convenient analysis. The `Installs` column was also cleaned to ensure proper analysis.

## Flowchart
The flowchart below illustrates the project's workflow:

![Flowchart](https://github.com/Romilj012/Predicting-the-Success-Rate-of-the-Upcoming-Mobile-Application-using-the-Google-Playstore-Dataset/blob/main/Screenshot%202023-05-25%20at%204.42.02%20PM.png)

## Algorithm
Multiple machine learning algorithms were employed to predict the rating of mobile applications, including Logistic Regression and Random Forest Classifier. The algorithms were compared to determine the best-performing one under specific conditions. Additionally, a recommendation system was developed to recommend the top 15 apps from a given genre based on weighted ratings.

## Results
The project's results include confusion matrices for decision tree, logistic regression, random forest, and tuned random forest algorithms. The confusion matrices provide insights into the classification performance. The project also recommends the top 15 apps using the recommendation system.

**Decision Tree Confusion Matrix**
![Decision Tree Confusion Matrix](https://github.com/Romilj012/Predicting-the-Success-Rate-of-the-Upcoming-Mobile-Application-using-the-Google-Playstore-Dataset/blob/main/Decision%20Con%20Matrix.png)

**Logistic Regression Confusion Matrix**
![Logistic Regression Confusion Matrix](https://github.com/Romilj012/Predicting-the-Success-Rate-of-the-Upcoming-Mobile-Application-using-the-Google-Playstore-Dataset/blob/main/logistic%20reg%20confusion%20matrix.png)

**Random Forest Confusion Matrix**
![Random Forest Confusion Matrix](https://github.com/Romilj012/Predicting-the-Success-Rate-of-the-Upcoming-Mobile-Application-using-the-Google-Playstore-Dataset/blob/main/random%20forest%20confusion%20matrix%20.png)

**Random Forest Confusion Matrix with Tuning**
![Random Forest Confusion Matrix with Tuning](https://github.com/Romilj012/Predicting-the-Success-Rate-of-the-Upcoming-Mobile-Application-using-the-Google-Playstore-Dataset/blob/main/Random%20Forest%20Con%20Ma%20with%20tuning.png)

**1. Low** shows apps not so popular 
**2. Medium** shows apps intermediate popular
**3. High** shows apps which are extremely popular

**Recommending Top 15 Apps using Recommendation System**
![Recommending Top 15 Apps using Recommendation System](https://github.com/Romilj012/Predicting-the-Success-Rate-of-the-Upcoming-Mobile-Application-using-the-Google-Playstore-Dataset/blob/main/Screenshot%202022-12-16%20at%2010.32.00%20PM.png)

## References
- [Google Playstore Apps Dataset](https://www.kaggle.com/datasets/gauthamp10/google-playstore-apps)
- [Creating Dataset for Sentiment Analysis by Scraping Google Play App Reviews](https://towardsdatascience.com/create-dataset-for-sentiment-analysis-by-scraping-google-play-app-reviews-using-python-ceaaa0e41c1)
- [Google Playstore Dataset EDA](https://github.com/vibhuti03/Google-Playstore-Dataset-EDAe)
- [Getting Things Done with Pytorch](https://github.com/curiousily/Getting-Things-Done-with-Pytorch)

Please refer to the project documentation and code for more detailed information and implementation details.

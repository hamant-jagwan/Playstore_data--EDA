# Exploratory Data Analysis on Google Play Store Dataset
<p align="center"> 
<img src="https://cdn.dribbble.com/users/2991/screenshots/1676747/media/126501a553d53578f1e056007f16f319.gif"  width="500" height="400" alt="GIF">
</p>


## Alternative URL
https://nbviewer.org/github/hamant-jagwan/playstore_data--EDA/blob/main/CAPSTONE_PROJECT_1_EDA.ipynb

## Introduction
    The Play Store apps data has enormous potential to drive app-making businesses to success. Actionable     
    insights can be drawn for developers to work on and capture the Android market. Each app(row) has values 
    for category, rating, size, and more. Another dataset contains customer reviews of the android apps. So, 
    we are Exploring and analysing the data to discover key factors responsible for app engagement and success.
## Data Set
    1. App - It tells us about the name of the application with a short description (optional).
    2. Category - It gives the category to the app.
    3. Rating - It contains the average rating the respective app received from its users.
    4. Reviews - It tells us about the total number of users who have given a review for the application.
    5. Size - It tells us about the size being occupied the application on the mobile phone.
    6. Installs** - It tells us about the total number of installs/downloads for an application.
    7. Type - IIt states whether an app is free to use or paid.
    8. Price - It gives the price payable to install the app. For free type apps, the price is zero.
    9. Content Rating - It states whether or not an app is suitable for all age groups or not.
    10. Genres - It tells us about the various other categories to which an application can belong.
    11. Last Updated - It tells us about the when the application was updated.
    12. Current Ver - It tells us about the current version of the application.
    13. Android Ver - It tells us about the android version which can support the application on its platform.

## Technologies Used
## The analysis was performed using Python 3.8, and the following libraries: 
    1. pandas 
    2. NumPy 
    3. matplotlib 
    4. seaborn. 

## Methodology
       The following steps were taken to perform the EDA on the data set:
       1. Data Cleaning
       2. Data Exploration & Feature Engineering
       3. Data Visualization
       4. Data Insight
    
## Data cleaning
    The dataset was cleaned by removing duplicates and null values.
    1. Android Ver: There are a total of 3 NaN values in this column.
    2. Current Ver: There are a total of 8 NaN values in this column.
    3. Type: There is only one NaN value in this column.
    4. Rating: This column contains 1470 NaN values.

## Data exploration & Feature Engineering 
    The dataset was explored by analyzing the distribution of app categories, ratings, reviews, installs,  and price.
    1. Handling the duplicates in the App column
    2. Changing the datatype of the Last Updated column from string to datetime.
    3. Changing the datatype of the Price column from string to float.
    4. Converting the values in the Installs column from string datatype to integer datatype.
    5. Converting the values in the Size column to the same unit of measure(MB).
    6. Converting the datatype of values in the Reviews column from string to int.
    7. Data Exploration--Univariate & Bivariate Analysis

## Data visualization
    The insights gained from the exploration were visualized using various plots such as histograms, scatter plots, and box plots.
    1. Correlation Heatmap
    2. Pie chart: What is the ratio of number of Paid apps and Free apps?
                  Which category of Apps from the Content Rating column are found more on playstore ?
    3. Histogram:  Top categories on Google Playstore?
                   Which category App's have most number of installs?
                   Average rating of the apps
                   What are the Top 10 installed apps in any category?
                   Top apps that are of free type.
                   Top apps that are of paid type.
                   Distribution of apps based on its size
      Data Visualization on User Reviews:
      1. Pie Chart:  Percentage of Review Sentiments
      2. Histogram:  Apps with the highest number of positive reviews
                     Apps with the highest number of negative reviews.
                     Histogram of Subjectivity
      3. Scatterplot: Is sentiment_subjectivity proportional to sentiment_polarity?
    
## Results
    1. Percentage of free apps = ~92%
    2. Percentage of apps with no age restrictions = ~82%
    3. Most competitive category: Family
    4. Category with the highest average app installs: Game
    5. Percentage of apps that are top rated = ~80%
    6. Family, Game and Tools are top three categories having 1906, 926 and 829 app count.
    7. Tools, Entertainment, Education, Buisness and Medical are top Genres.
    8. 8783 Apps are having size less than 50 MB. 7749 Apps are having rating more than 4.0 including both type of apps.
    9. There are 20 free apps that have been installed over a billion times.
    10. Minecraft is the only app in the paid category with over 10M installs. This app has also produced the most revenue only from the installation fee.
    11. Category in which the paid apps have the highest average installation fee: Finance
    12. The median size of all apps in the play store is 12 MB.
    13. The apps whose size varies with device has the highest number average app installs.
    14. The apps whose size is greater than 90 MB has the highest number of average user reviews, ie, they are more popular than the rest.
    15. Helix Jump has the highest number of positive reviews and Angry Birds Classic has the highest number of negative reviews.
    16. Overall sentiment count of merged dataset in which Positive sentiment count is 64%, Negative 22% and Neutral 13%.

## Conclusion
    In this project of analyzing play store applications, we have worked on several parameters which would help companies to do well in launching their apps on the play store.
    
    In the initial phase, we focused more on the problem statements and data cleaning, in order to ensure that we give them the best results out of our analysis.
    
    Companies need to focus more on:
    
    1. Developing apps related to the least categories as they are not explored much. Like events and beauty.
    2. Most of the apps are Free, so focusing on free app is more important.
    3. Focusing more on content available for Everyone will increase the chances of getting the highest installs.
    4. They need to focus on updating their apps regularly, so that it will attract more users.
    5. They need to keep in mind that the sentiments of the user keep varying as they keep using the app, so they should focus more on users needs and features.


## Acknowledgements
    This project was completed as part of a data science course at AlmaBetter. 
    Special thanks to the course instructors for their guidance and support.

## How to Run
    To run the analysis, you can clone the GitHub repository to your local machine and run the Google colab notebook. Make sure you have the necessary dependencies are installed.

# **Play Store App Review Analysis** 

Project Type - EDA

Contribution - Individual

![image](https://user-images.githubusercontent.com/109869652/215673107-1efd1002-a6ef-487e-9ed7-bee0749cd271.png)

# **About Project**

Data from Google Play Store can provide valuable insights for app developers and businesses to improve their app offerings and marketing strategies. By analyzing user ratings, reviews, and download numbers, developers can identify areas for improvement and optimize their app to drive growth and success.
In this notebook, I'm gonna analyze Google Play Store datas. While I was analyzing the data, I used Python.
* **playstore data.csv:** contains all the details of the applications on Google Play. There are 13 features that describe a given app.
* **user_reviews.csv**: contains 100 reviews for each app, most helpful first. The text in each review has been pre-processed and attributed with three new features: Sentiment (Positive, Negative or Neutral), Sentiment Polarity and Sentiment Subjectivity.

# **Project Objective**
The objective of the Play Store App Review Analysis is to gain insights into user opinions and feedback for a particular mobile app available on the Google Play Store. The analysis aims to identify common themes and trends in the app reviews, such as user satisfaction, key features that users like or dislike, and potential areas for improvement. The outcome of the analysis will be used to inform the app development team's decisions and strategies to enhance the app's overall user experience and increase user satisfaction.

# **Problem Statements**
1. What are the top categories on Play Store?
2. Are majority of the apps Paid or Free?
3. How importance is the rating of the application?
4. Which categories from the audience should the app be based on?
5. Which category has the most no. of installations?
6. How does the count of apps varies by Genres?
7. How does the last update has an effect on the rating?
8. How are ratings affected when the app is a paid one?
9. How are reviews and ratings co-related?
10. Lets us discuss the sentiment subjectivity.
11. Is subjectivity and polarity proportional to each other?
12. What is the percentage of review sentiments?
13. How is sentiment polarity varying for paid and free apps?
14. How Content Rating affect over the App?
15. Does Last Update date has an effects on rating?

# **What is Exploratory Data Analysis?**
Exploratory Data Analysis (EDA) is an approach to analyzing and understanding a dataset through visual and statistical methods to summarize its main features and identify relationships and patterns in the data. It's a preliminary step to more formal modeling and hypothesis testing and helps to formulate hypothesis and inform feature engineering.

# **Dataset Information:**

1. **App** - It tells us about the name of the application with a short description (optional).
2. **Category** - It gives the category to the app.
3. **Rating** - It contains the average rating the respective app received from its users.
4. **Reviews** - It tells us about the total number of users who have given a review for the application.
5. **Size** - It tells us about the size being occupied the application on the mobile phone.
6. **Installs** - It tells us about the total number of installs/downloads for an application.
7. **Type** - IIt states whether an app is free to use or paid.
8. **Price** - It gives the price payable to install the app. For free type apps, the price is zero.
9. **Content Rating** - It states whether or not an app is suitable for all age groups or not.
10. **Genres** - It tells us about the various other categories to which an application can belong.
11. **Last Updated** - It tells us about the when the application was updated.
12. **Current Ver** - It tells us about the current version of the application.
13.**Android Ver** - It tells us about the android version which can support the application on its platform.

# **Cleaning of the data**
Data cleaning is the process of identifying and correcting errors, inconsistencies, and inaccuracies in a dataset, in order to make it usable for analysis and decision-making. This process includes identifying missing or invalid data, removing duplicates, handling missing values, correcting inconsistent data, filtering irrelevant data, transforming data into a usable format, and storing the cleaned data in a new file or database.

**steps:-**

* Identify missing or invalid data
* Remove duplicates
* Handle missing values (e.g. imputation)
* Correct inconsistent data (e.g. standardize units)
* Filter irrelevant data
* Transform data into a usable format
* Store the cleaned data in a new file or database.

# **Data Visualization**

Data visualization is the representation of data in a graphical or pictorial format, such as charts, graphs, maps, and images. The goal of data visualization is to make complex data more accessible, understandable, and actionable by transforming it into a visual format that highlights patterns, trends, and insights. Data visualization can be used in various fields, including business, science, and journalism, to support data-driven decision-making and communicate findings effectively.

# **Analysis Summary**
In this project of analyzing play store applications, we have worked on several parameters which would help App Developers to do well in launching their apps on the play store.

In the initial phase, we focused more on the problem statements and data cleaning, in order to ensure that we give them the best results out of our analysis.

App Developers needs to focus more on:
1. Developing apps related to the least categories as they are not explored much. Like events and beauty.
2. Most of the apps are Free, so focusing on free app is more important.
3. Focusing more on content available for Everyone will increase the chances of getting the highest installs.
4. They need to focus on updating their apps regularly, so that it will attract more users.
5. They need to keep in mind that the sentiments of the user keep varying as they keep using the app, so they should focus more on users needs and features.

**1.Rating**

Most of the apps have rating in between 4 and 5.

Most numbers of apps are rated at 4.3

Categories of apps have more than 4 average rating.item

 **2.Size**

Maximum number of applications present in the dataset are of small size.

**3.Installs**

Majority of the apps come into these three categories, Family, Game, and Tools.

Maximum number of apps present in google play store come under Family, Game and tools but as per the installation and requirement in the market plot, scenario is not the same. Maximum installed apps comes under Game, Communication, Productivity and Social.

Subway Surfers, Facebook, Messenger and Google Drive are the most installed apps.

**4.Type(Free/Paid)**

About 92% apps are free and 8% apps are of paid type.

The category ‘Family’ has the highest number of paid apps.

Free apps are installed more than paid apps.

The app “I’m Rich — Trump Edition” from the category ‘Lifestyle’ is the most costly app priced at $400

**5.Content Rating**

Content having Everyone only has most installs, while unrated and Adults only 18+ have less installs.

**6.Reviews**

Number of installs is positively correlated with reviews with correlation 0.64.
Sentiment Analysis

**7.Sentiment** 

Most of the reviews are of Positive Sentiment, while Negative and Neutral have low number of reviews.

**8.Sentiment Polarity / Sentiment Subjectivity**

Collection of reviews shows a wide range of subjectivity and most of the reviews fall in [-0.50,0.75] polarity scale implying that the extremely negative or positive sentiments are significantly low.
Most of the reviews show a mid-range of negative and positive sentiments.

Sentiment subjectivity is not always proportional to sentiment polarity but in maximum number of case, shows a proportional behavior, when variance is too high or low.

Sentiment Polarity is not highly correlated with Sentiment Subjectivity.

#  **Challenges**

* Handling large volume of data: The number of app reviews can be overwhelming, and processing such large amounts of data can be a challenge.
* Major challenge was data cleaning.

* Dealing with subjective opinions: User opinions and feedback can be subjective, making it challenging to reach objective conclusions.

# **Future Work**

* We can explore the correlation between the size of the app and the version of Android on the number of installs.
* Machine learning can help us to deploy more insights by developing models which can help us interpret even more better. We have left this as future work as this is something where we can work on.
* Improving sentiment analysis techniques: There is room for improvement in sentiment analysis techniques to accurately capture the sentiment expressed in app reviews.

* Incorporating additional data sources: Other data sources such as demographic information about app users, usage data, and device information could be incorporated to provide a more complete picture of the app's user base and performance.

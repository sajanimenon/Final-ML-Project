# Sales-Prediction
Implementation of Advertisement dataset

  About Data :
  
  Dataset link: https://www.kaggle.com/purbar/advertising-data
  Dataset has 3 features TV,radio,newspaper and one label Sales.
  The number of observations are 200. 
  First 3 featuers are the advertisements shown in each medium (tv, newspaper or radio) and 4th label i.e sales is the number of sales after the advertisement. 
  
  Goal:
  
  The goal is to find the find the realtionship between advertisement and sales, and to predict the sales for a particular number of advertisement in each medium. 

  
  I used Scikit-Learn, Pandas and numpy for this project.

 Step 1 : Find relationship of each feature with label respectively by making a pairplot using seaborn library .
 Step 2: Use pandas correlation function to find the correlation between each feature all together
 
 Observation:
 TV advertisment data was more linear, had the biggest impact on sales, than radio and newspapaer. 
 Newspaper,infact had the lowest affect on the sales.
 
 
 Step 3:  Predict Sales using linear regression (Split data into train and test)
 
 - used linear regression model to predict the sales using different combination of features (considering the result we got in last of finding realtionship between features). 
 
 Step 4: Use a metric to calculate Error
 
 - I ran linear regression 1000 times and calculated the average mean squared error (used it as a metric to calculate error) which was around 1.7 , I noticed that when I used only TV and radio features to predcit sales, I got better result than when used all features. 
 
 Step 5 : Cross Validation
 
 Then I tried cross validation technique to find the best features for predicting the most accurate sales. I got 1.69 root mean squared error when I used all features and 1.67 when i used only tv and radio. 

Observation : Using 2 features provides a better prediction , so to generalize the more the number of features more the error.

Dataset link: https://www.kaggle.com/purbar/advertising-data


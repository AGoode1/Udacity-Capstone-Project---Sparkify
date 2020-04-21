# Udacity-Capstone-Project---Sparkify
Capstone project for Udacity's Data Scientist Nano-Degree. Build a machine learning model in PySpark. 

Blog post for this project can be found at the link: https://medium.com/@andrew.goode_70135/building-an-ml-model-in-pyspark-7d270ca59444

Sparkify.ipynb: Contains the entire code package for imorting data, cleaning, data exploration, feature engineering and modelling. 

Data Source: Data used was a small subset of the full Sparkify data made available by Udacity. The reason for this is that this project is run in a Jupyter notebook. To use the full dataset a cluster must be deployed on the cloud.
Whilst this project utilises PySpark libraries, it does not utilize the clustering capabilities that Spark allows. 
A future addition onto this work may deploy a larger portion of the dataset, using a cluster. 

Motivation: As part of the Udacity Data Scientist nano-degree program, I was required to investigate a dataset. One option was to use PySpark to build a prediction model on a given data-set, which is what I have opted to do. 

The dataset: The dataset contains user activity of a fictitious music streaming service called Sparkify. Each row is a user interaction such as playing a new song, adding a song to a playlist etc. The label of interest is whether or not a customer closes their account (Churn). The model aims to predict which users are likely to cancel their account. 

Features developed: 1. Predictive actions (in "page" column) frequency in total, and over 1,2,3 and 4 latest weeks of data for a user. 
                    2. Gender
                    3. Membership status in the last row of data for a user (free or paid)
                    4. The average length of a session for a user
                    5. The ratio of songs played in the last week, compared to songs played in total over the last 4 weeks
                    
Models used: All mdoels were developed using the PySpark ML library.
             1. Logistic Regression
             2. Gradient Boosted Tree
             3. Decision Tree
             4. Random Forest

Model results: 1.Decision Tree (F1 Score: 0.50)
               2.Gradient Boosted Tree (F1 Score: 0.48)
               3.Random Forest (F1 Score: 0.30)
               4.Logistic Regression (F1 Score: 0.13)
            
                    
                    
                    

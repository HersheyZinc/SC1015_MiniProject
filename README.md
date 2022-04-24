# About

## Problem Definition: Is it possible to predict if a song will be popular? 

Our project utilised the Spotify Million Playlist Dataset obtained from https://www.aicrowd.com/challenges/spotify-million-playlist-dataset-challenge/dataset_files and Spotify’s web API to extract key features of the songs such as danceability, energy, key, loudness, mode, speechiness, acousticness, instrumentalness, liveness, valence, tempo, durection_ms, name, popularity, artist and genre. 



##### 👦🏻👩🏻👦🏻Members: 


1. Chua Jing Jie, Justin @Whatjustin

2. Jessie Ang @jessieeang

3. Lim Zhe Xun @HersheyZinc


## 📝📝Content

##### 🎵🎵🎵Importing the Dataset:


- Using Spotify API

- Cleaning null/duplicate data



##### 📊📊Exploratory Data Analysis:


- Univariate Pair Plot

- Univariate Box Plot

- Univariate Violin Plot

- Univariate Histogram 




##### 🧹🧹Data Cleaning: 



- ‘Key’ , ‘Artist’ and ‘Mode’ were dropped as variables 

- Songs with ‘Popularity’ score of zero were dropped 

- One-Hot encoding for genres




##### 📈📉Advanced EDA:


1. Correlation Heatmap

2. Bar Plot

3. Pair Plot



##### 🔧🔧Tuning Techniques: 


- Balanced accuracy metrics

- Grid Search



##### 💻💻Machine Learning Models (Balance Accuracy Score taken as metric): 

1. Decision Tree

2. Random Forest Classifier

3. K-Nearest Neighbours

4. Logistic Regression 

5. Gradient Boosting



## 🔍🔍Conclusions: 

Random Forest Classifier was the best model as it yielded the highest Balance Accuracy Score of 60.9% . However, 60.9% is still considered low and cannot be considered reliable. A justification for why the Balanced Accuracy Scores across all models were prevailingly low could be due to insufficient independent variables and weak dependent variables, along with a prevailing large disproportion between the number of popular songs and not popular songs despite us dropping songs with zero popularity causing our data to be imbalance despite us adopting measures to mitigate that problem. 


Some possible improvements could be increasing the number of popular songs within the data to ensure greater balance. Adopting over or under sampling could also have a positive effect on our models if used in tandem. More independent variables should also be identified such as ‘current trends in music’ and  ‘social media’. Another possible variable could be ‘Artist’ as despite us dropping to variable so as to not introduce bias within the data, ‘Artist’ is theoretically a good metric for the popularity of a song. Furthermore, we noted that the popularity variable provided by Spotify only reflects a track’s current popularity. As such, negating the success of old songs that are past their prime. A solution to this might be to use a song’s lifetime streams as a metric for popularity or break down popularity into more subsets such as ‘region’ or ‘time period’. This would allow us to more accurately determine a song’s overall popularity regardless of the current trends.

## Online references : 


https://www.investopedia.com/articles/investing/120314/spotify-makes-internet-music-make-money.asp 

https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html 

sklearn.tree.DecisionTreeClassifier — scikit-learn 1.0.2 documentation

3.3. Metrics and scoring: quantifying the quality of predictions — scikit-learn 1.0.2 documentation

https://www.analyticsvidhya.com/blog/2018/03/introduction-k-neighbours-algorithm-clustering/ 

sklearn.ensemble.RandomForestClassifier — scikit-learn 1.0.2 documentation

https://machinelearningmastery.com/gentle-introduction-gradient-boosting-algorithm-machine-learning/

https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.GradientBoostingClassifier.html 

https://towardsdatascience.com/predicting-popularity-on-spotify-when-data-needs-culture-more-than-culture-needs-data-2ed3661f75f1#:~:text=According%20to%20Spotify%2C%20%E2%80%9Cpopularity%20is,a%20lot%20in%20the%20past.%E2%80%9D 

7 Spotify Statistics that can help your business [2022] (rockcontent.com)


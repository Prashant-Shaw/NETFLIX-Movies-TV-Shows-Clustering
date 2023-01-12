# NETFLIX-Movies-TV-Shows-Clustering
Project Name - Netflix Movies & TV Shows Clustering

Project Status - Complete

Language Used - Python with Pandas, Numpy, Matplotlib, Seaborn, Ploty, SKlearn, nltk and scipy libraries

Problem Statement -
This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.
The goal of this project is to classify/group the Netflix shows into certain clusters such that the shows within a cluster are similar to each other and the shows in different clusters are dissimilar to each other.

Appraoch - 
To explore the dataset and extract useful insights from the dataset. We will be diving the dataset into several groups / clusters using unsupervised ML - K Means clustering and Hierarchical clustering. In the last we will be building a recommender system which will recommend movies/shows based on current liking.

Conclusion - 

* We have successfully implemented Unsupervised Machine learning algorithm where we have clustered the data on Netflix dataset. We have divided the dataset into several clusters.
* There are 7787 rows and 12 columns in the dataset.
* We performed data cleaning and EDA. From EDA we have following observations -
    * In the dataset around 69% of Movie is present and 31% of TV Show is present.
    * Christmas, World, Love, Man are some of the most words in the title.
    * US, India & UK are having the most production.
    * The majority of the shows on Netflix are for adults and for children above age 14.
    * International movies are having the highest count in the dataset.
    * Description of TV Shows contains more words like world, life, family, new, find, love etc. 
    * Description of Movie also contains more words like life, find, family, love etc similar to TV Shows.
* We found that over the years, Netflix has consistently focused on adding more shows in its platform. There is a decrease in number of movies added in the year 2020 as compared to year 2019 whereas the number of TV Shows have increased from 656 to 697 from year 2019 to year 2020.
* Number of TV Shows have increased more than 3 times also number of movies are increasing on year basis.
* We clustered the data based on the features - director, cast, country, genre, and description. The values in these attributes were tokenized, preprocessed, and then vectorized using TFIDF vectorizer.
* Through TFIDF Vectorization, we created a total of 20000 attributes.
* We used Principal Component Analysis (PCA) to handle the curse of dimensionality. 4000 components were able to capture more than 80% of variance, and hence, the number of components were restricted to 4000. 
* We have first used K-Means clustering for clustering the data. We used elbow method & Silhouette method to get the optimal value of k. With the optimal k as 9 from Silhouette score we have clusterred the data into 9 clusters.
* Then we have made the clusters using Agglomerative Hierarchical method where we have divided the dataset into 11 clusters after visualizing the dendogram.
* In the last a content based recommender system was built using cosine similarity. This system will recommend 10 shows/movies based on your current liking.


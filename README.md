# Netflix-Movies-and-TV-Shows-Clustering
Netflix is the world's largest online streaming service provider, with over 220 million subscribers as of 2022-Q2. It is crucial that they effectively cluster the shows that are hosted on their platform in order to enhance the user experience, thereby preventing subscriber churn.
# Problem Statement
This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.

In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.
# Dataset
The dataset is collected from Flixable which is a third-party Netflix search engine. This dataset consists of tv shows and movies available on Netflix as of 2019. It includes over 7787 records and 12 attributes. Each attribute is provide information about movies/TV shows. More details of the dataset can be found in the kaggle website.
# Approach
Problem Statement
Importing the Libraries and the Dataset
Understanding Data
Exploratory Data Analysis
Data Cleaning
Textual Data Preprocessing
Clusters Impelementation
Recommendation System.
Conclusions
# conclusions
In this project, we worked on a text clustering problem wherein we had to classify/group the Netflix shows into certain clusters such that the shows within a cluster are similar to each other and the shows in different clusters are dissimilar to each other.

The dataset contained about 7787 records, and 11 attributes. the most content is added to Netflix from october to january

* Documentaries are the top most genre in netflix which is fllowed by standup comedy and Drams and international movies
kids tv is the top most TV show genre in netflix

* most of the movies have duration of between 50 to 150

* highest number of tv_shows consistig of single season

* Those movies that have a rating of NC-17 have the longest average duration.

* When it comes to movies having a TV-Y rating, they have the shortest runtime on average

* unitated states has the highest number of content on the netflix ,followed by india

* india has highest number of movies in netflix

*30% movies released on Netflix.

* 70% movies added on Netflix were released earlier by different mode.

*We began by dealing with the dataset's missing values and doing exploratory data analysis (EDA).It was found that Netflix hosts more movies than TV shows on its platform, and the total number of shows added on Netflix is growing exponentially.

*Also, majority of the shows were produced in the United States, and the majority of the shows on Netflix were created for adults and young adults age group.

* It was decided to cluster the data based on the attributes: director, cast, country, genre, and description.

* The values in these attributes were tokenized, preprocessed, and then vectorized using TFIDF vectorizer.Through TFIDF Vectorization, we created a total of 20000 attributes.We used Principal Component Analysis (PCA) to handle the curse of dimensionality. 4000 components were able to capture more than 80% of variance, and hence, the number of components were restricted to 4000.

* firstly built clusters using the k-means clustering algorithm, and the optimal number of clusters came out to be 6. This was obtained through the elbow method and Silhouette score analysis.

* Then clusters were built using the Agglomerative clustering algorithm, and the optimal number of clusters came out to be 12. This was obtained after visualizing the dendrogram.

* A content based recommender system was built using the similarity matrix obtained after using cosine similarity. This recommender system will make 10 recommendations to the user based on the type of show they watched.

* In conclusion, Netflix clustering using machine learning algorithms such as k-means and agglomerative hierarchy analysis can provide valuable insights into user behavior and preferences. By grouping users into clusters based on their viewing habits and ratings, Netflix can better understand their customers and provide personalized recommendations.

* K-means clustering is a simple and efficient algorithm that can quickly group users into clusters based on their similarity. However, it requires specifying the number of clusters beforehand, which can be challenging. Agglomerative hierarchy analysis, on the other hand, does not require specifying the number of clusters beforehand and can create a hierarchy of clusters that provides additional insights into user behavior.

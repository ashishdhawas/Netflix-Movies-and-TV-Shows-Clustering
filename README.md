# Netflix-Movies-and-TV-Shows-Clustering

Project Summary -
In our project, Netflix Movies & TV Shows Clustering, we were able to analyse and perform an unsupervised Machine Learning Algorithm for the unlabelled datasets. The dataset we were provided with contains several columns and other numerical features. We were also asked two questions that could be answered from EDA.

The EDA was done extensively as we needed to derive good insights to support our claim and hypothesis. We were able to answer the two questions that followed along with the EDA, country-wise trend analysis on content and genre; and also to analyse if Netflix was focusing more on Shows rather than Movies.

After we performed EDA, both univariate and bivariate analysis, we have prepared our text columns by following basic text cleaning, stopwords removal, tokenisation and stemming. After the text columns were ready, we selected only features or words that were important using TF IDF Vectorisation and also reduced dimension.

The prepared text columns were clustered after selecting an optimal value from elbow plots. Finally, we used K Means to cluster our dataset into 6 distinct clusters and we were also able to encode or label the dataset accordingly.

Subsets of dataset formed from clustering were analysed and word clouds were plotted, after which we used interactive Plotly visualisation to represent the cluster.

Finally, a simple recommendation system was also tried out, the future scopes for the projects were also identified.

Conclusions:
In this project, we worked on a text clustering problem wherein we had to classify/group the Netflix shows into certain clusters such that the shows within a cluster are similar to each other and the shows in different clusters are dissimilar to each other.

The dataset contained about 7787 records, and 11 attributes.

We began by dealing with the dataset's missing values and doing exploratory data analysis (EDA).

It was found that Netflix hosts more movies than TV shows on its platform, and the total number of shows added on Netflix is growing exponentially. Also, majority of the shows were produced in the United States, and the majority of the shows on Netflix were created for adults and young adults age group.

It was decided to cluster the data based on the attributes: director, cast, country, genre, and description. The values in these attributes were tokenized, preprocessed, and then vectorized using TFIDF vectorizer.

Through TFIDF Vectorization, we created a total of 20000 attributes.

We used Principal Component Analysis (PCA) to handle the curse of dimensionality. 4000 components were able to capture more than 80% of variance, and hence, the number of components were restricted to 4000.

We first built clusters using the k-means clustering algorithm, and the optimal number of clusters came out to be 6. This was obtained through the elbow method and Silhouette score analysis.

Then hierarchical clusters were built using the Agglomerative clustering algorithm, and the optimal number of clusters came out to be 12. This was obtained after visualizing the dendrogram.

A content based recommender system was built using the similarity matrix obtained after using cosine similarity. This recommender system will make 10 recommendations to the user based on the type of show they watched.


# Hybrid-Recommendation-System
With the development of technology, our habits are also changing. Mostly used in digital space, eBay, Amazon, Alibaba, etc. As such, most of today’s E-Commerce sites use their own proprietary recommendation algorithms to better serve customers with the products they have to like. There are many examples such as Netflix’s movies, Spotify’s music, Facebook recommending friends, product recommendations of Amazon, etc. One of the reasons why these companies are so popular can be shown that their business structures are based on recommendation systems.

What is Recommendation System?
A recommendation engine is a filtering system that analyzes this data from heterogeneous sources belonging to different users and produces solutions to anticipate their interest and recommend the relevant products to the right users accordingly. However, the Recommendation system is a machine learning algorithm that offers users suggestions on what they might like based on their past preferences.

Most recommender systems now use a hybrid approach, combining collaborative filtering, content-based filtering, and other approaches.

There are three main types of techniques for Recommendation engines:

Collaborative filtering
Content-Based Filtering
Hybrid Recommendation Systems
Netflix is a good example of the use of hybrid recommender systems. The website makes recommendations by comparing the watching and searching habits of similar users (i.e., collaborative filtering) as well as by offering movies that share characteristics with films that a user has rated highly (content-based filtering).

One of the events that energized research in recommender systems was the Netflix Prize. We will discuss these topics with the data set discussed in this contest.

The dataset I used here comes directly from Netflix. It consists of 4 text data files, each file contains over 20M rows, i.e. over 4K movies and 400K customers. Altogether over 17K movies and 500K+ customers!


For example, we initially select a random user and focus on the movies that that user watches.


the number of movies watched by the user we determined is 455.

Collaborative Recommendation System
Collaborative recommendation systems aggregate ratings or recommendations of objects, recognize partnerships between users based on their ratings and generate new recommendations based on user-to-user comparisons. Usually, it is based on collecting and analyzing information about the user’s behavior, activities, or preferences and predicting what they will like based on similarity with other users. Collaborative systems analyze user and/or item similarities.

Determining the most similar users to the user to be recommended We look at the relationship (similarity) between the user and the users, which we determined by correlation.

Further, there are several types of collaborative filtering algorithms:


image
1- User-User Collaborative Filtering: It is based on searching for similar customers and offering suggestions based on similar ones. This algorithm is very effective but takes a lot of time and resources.


Determined the users who watch at least 60 percent (subject to change) of the movies the user watches.


We bring together users who watch the same movies with the user. (most similar users to the user to be recommended)

2-Item-Item Collaborative Filtering: It is a type of recommendation method that searches for similar items based on items users have previously liked or positively interacted with. It requires fewer resources and time compared to user-user collaboration filtering.


We can recommend other movies watched by users who are at least 60 percent similar to the user we selected.
Content-Based Filtering System
The filtering system is based on a single user’s interactions and preferences. It is based on metadata gathered from a user’s history and interactions. A Content-Based suggestion learns a profile of the new user’s interests based on existing properties in the objects the user has graded. The algorithms are such that they suggest similar items to users that they have liked in the past or are currently viewing.

To create a user profile, the system mostly focuses on two types of information:

A model of the user’s preference.
A history of the user’s interaction with the recommender system.
The more information the user provides, the higher the accuracy.


image
Hybrid Recommender Systems
We can make recommendations according to the last watched and high-rated movie titles of the user.

Most recommender systems now use a hybrid approach, combining collaborative filtering, content-based filtering, and other approaches.

The hybrid recommendation system can be used to overcome common problems such as data

insufficiency. Some hybridization techniques include:

Weighted: Combining the score of different recommendation components numerically.


Switching: Choosing among recommendation components and applying the selected one.

Mixed: Recommendations from different recommenders are presented together to give the recommendation.

Feature Combination: Features derived from different knowledge sources are combined and given to a single recommendation algorithm.

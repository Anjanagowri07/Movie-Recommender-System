MOVIES RECOMMENDATION

Abstract: 
Recommender systems are aimed at helping the users to find the relevant items based on their interests by providing some suggestions. There are many types of recommendation systems out of which we chose content-based recommendation system for our project. Content-based recommendations are best suited when there is sufficient data about the item but not the user. User profiles are created and the description of the item is given, based on which item similarities are calculated and suggested to the users. This project investigates how movie overviews, taglines, popularity and ratings are used to suggest movies that are most similar to a given movie. This is done using the concepts of cosine similarity, TF-IDF measures, content-based recommendation model.

Introduction: 
Comparing to the previous years, the demand of the OTT platforms has increased rapidly. People started preferring Netflix, Amzon Prime, etc. to watch movies in their homes. Each and every user has a profile and their history is recorded in order to note the preference of the particular user. The OTT platforms suggest movies to the user based on their interests. They use recommendation systems through which previous data of the user like the ratings, popularity of the movie is recorded and suggestions of movies for a particular user are made.  

Related work: 
In content-based filtering, the items are best described using the keywords and a user profile is built to store the information on the type of the item the user prefers or searches. Various items are compared with the items that are of the user’s interests earlier i.e., either the items that are given good ratings by the user or those that are most used or purchased, and the best-matching items are suggested. In the different research papers, we have gone through, the recommendations are mostly made based on the user’s previous history, ratings, likes and the customer behavior.



Methodology:
The movies are suggested to the users based on the content of the movie they watched previously. The overview and taglines of the movies are combined into descriptions. Now, we get the TF-IDF score of the text from the descriptions of the movie. This vector is used in finding the cosine similarity. Now we recommend top 10 movies for each and every movie depending upon the user’s profile. Also, popularity and rating of the movies are considered and sorted accordingly within the already suggested movies.

Experimental Discussion:
Sklearn and its functions (tf-idf vectorizer linear kernel): Term frequency-inverse document frequency is a text vectorizer that transforms the text into a usable vector. We used the tf-idf vectorizer to convert the textual data into tf-idf vectors upon which we compute the cosine similarity to obtain the similarity based in this computation. We did all of the said computation on the data frame “description” which we obtain using the attributes ‘tagline’ and ‘overview’, which contain the textual data describing the movie it belongs to. 
Conclusion:
This project recommends the users few movies whenever they watch a movie based on the interest and behavior of that particular user. This is done using a recommendation system. We have used TF-IDF and cosine similarities in order to get the similar movie recommendations. The overviews, taglines, popularity and ratings of the movie watched by the user are considered and new movies are suggested based on this content. Further developments can be made by considering only the information based on profile ratings and the user’s previous history which is known as collaborative filtering.



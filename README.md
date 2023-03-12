### Collaborative filtering with matrix factorization for movie recommendation system

#### I am using user rated movies data and predict ratings for given user. Then after sorting can recommend top n movies to user based on his previous rated movies. Used matrix factorization for collaborative filtering for this analysis.

Below use cases can be for this analysis.
- Can recommend movies to use on home page of website or app based on his rated movies.
- Can send email to user for movies he might be interested in based on his previous ratings.
- Users with similar rattings can get recommendations based on other users with similar interests.

Files in repo and their details.
- "Exploratory Analysis - Collaborative.ipynb" this file is for different graphs and other stats about data we used for analysis.
- "Collaborative filtering with matrix factorization for movie recommendation system.ipynb" as name suggests this file is for main model to recommend movies based on user ratings. I have used scipy and surprise libraries for analysis.

I am "hetrec2011-movielens-2k" dataset for this analysis. Data is included in data folder of this repo. Details of dataset are below.
This dataset is an extension of MovieLens10M dataset, published by GroupLeans research group. http://www.grouplens.org

---------------
Data statistics
---------------

    2113 users
   10197 movies

  855598 ratings
         avg. 404.921 ratings per user
         avg. 84.637 ratings per movie


-----
Files
-----

   * movies.dat
   
   	This file contains information about the movies of the database.
   	
   	The original movie information -title and year- available at MovieLens10M dataset 
   	has been extended with public data provided in IMDb and Rotten Tomatoes websites:
   	   - Titles in Spanish
   	   - IMDb movie ids
   	   - IMDb picture URLs
           - Rotten Tomatoes movie ids
           - Rotten Tomatoes picture URLs
           - Rotten Tomatoes (all/top) critics' ratings, avg. scores, numbers of 
             reviews/fresh_scores/rotten_scores
           - Rotten Tomatoes audience' avg. ratings, number of ratings, avg. scores
   
   * user_taggedmovies.dat - user_taggedmovies-timestamps.dat
   
        These files contain the tag assignments of the movies provided by each particular user.
        
        They also contain the timestamps when the tag assignments were done.
   
   * user_ratedmovies.dat - user_ratedmovies-timestamps.dat
   
        These files contain the ratings of the movies provided by each particular user.
        
        They also contain the timestamps when the ratings were provided.

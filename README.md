# ZEE5

## Business Problem
Create a Recommender System to show personalized movie recommendations based on ratings given by a user and other users similar to them in order to improve user experience.

## Data Dictionary:
=========================================================================

### RATINGS FILE DESCRIPTION
============================
• All ratings are contained in the file "ratings.dat" and are in the following format:UserID::MovieID::Rating::Timestamp
   • UserIDs range between 1 and 6040
   • MovieIDs range between 1 and 3952
   • Ratings are made on a 5-star scale (whole-star ratings only)
   • Timestamp is represented in seconds
   • Each user has at least 20 ratings
### USERS FILE DESCRIPTION
==========================

•  User information is in the file "users.dat" and is in the following format: UserID::Gender::Age::Occupation::Zip-code
•  All demographic information is provided voluntarily by the users and is not checked for  accuracy.
•  Only users who have provided some demographic information are included in this data set.
• Gender is denoted by a "M" for male and "F" for female
• Age is chosen from the following ranges:
    o 1: "Under 18"
    o 18: "18-24"
    o 25: "25-34"
    o 35: "35-44"
    o 45: "45-49"
    o 50: "50-55"
    o 56: "56+"
    • Occupation is chosen from the following choices:
    o 0: "other" or not specified
    o 1: "academic/educator"
    o 2: "artist"
    o 3: "clerical/admin"
    o 4: "college/grad student"
    o 5: "customer service"
    o 6: "doctor/health care"
    o 7: "executive/managerial"
    o 8: "farmer"
    o 9: "homemaker"
        o 10: "K-12 student"
        o 11: "lawyer"
        o 12: "programmer"
        o 13: "retired"
        o 14: "sales/marketing"
        o 15: "scientist"
        o 16: "self-employed"
        o 17: "technician/engineer"
        o 18: "tradesman/craftsman"
        o 19: "unemployed"
        o 20: "writer"
### MOVIES FILE DESCRIPTION
===========================

• Movie information is in the file "movies.dat" and is in the following format: MovieID:: Title::Genres
• Titles are identical to titles provided by the IMDB (including year of release)
• Genres are pipe-separated and are selected from the following genres:
    o Action
    o Adventure
    o Animation
    o Children's
    o Comedy
    o Crime
    o Documentary
    o Drama
    o Fantasy
    o Film-Noir
    o Horror
    o Musical
    o Mystery
    o Romance
    o Sci-Fi
    o Thriller
    o War
    o Western
## Questionnaire:
=========================================================================

   1. Users of which age group have watched and rated the most number of movies?
   2. Users belonging to which profession have watched and rated the most movies?
   3. Most of the users in our dataset who’ve rated the movies are Male. (T/F)
   4. Most of the movies present in our dataset were released in which decade?
   1. 70s b. 90s c. 50s d.80s
   5. The movie with maximum no. of ratings is ___.
   6. Name the top 3 movies similar to ‘Liar Liar’ on the item-based approach.
   7. Mention the RMSE and MAPE that you got while evaluating the Matrix 
   Factorization model.
    
## Concepts Tested:
=========================================================================

• Recommender Engine
• Collaborative Filtering (Item-based & User-based Approach)
• Pearson Correlation
• Nearest Neighbors using Cosine Similarity
• Matrix Factorization

## Project Accomplishments and Process Overview
=========================================================================

  • Reading the data files, formatting them into a proper workable format and merging the data files into one single dataframe
    Eg: pd.read_fwf('../input/zeemovie/movies.dat', encoding='ISO-8859-1'
  • Performing exploratory data analysis like checking the structure & characteristics of the dataset and cleaning the data
  • Performing feature engineering steps type conversions and deriving new features like ‘Release Year’
  • Visualizing the data with respect to different categories to get a better understanding of the underlying distribution
  • Grouping the data in terms of Average Rating and No. of Ratings given
  • Creating a pivot table of movie titles & user id and imputing the NaN values with a suitable value
  • Follow the Item-based approach and
      o Pearson Correlation
      o Cosine Similarity
  • Matrix Factorization
      o Evaluate the model’s performance using RMSE and MAPE
  • Embeddings for item-item and user-user similarity
      o Re-design the item-item similarity function to use MF embeddings (d=4) 
      instead of raw features
      o Similarly, do this for user-user similarity


    
    

# Movie-Recommendation-System
## Project Overview
A Movie Recommendation System built on the MovieLens dataset containing 100,000 movie ratings. The repository includes Jupyter notebooks demonstrating implementation and evaluation, along with source code, data files, and setup instructions. Contributions are welcome under the MIT License.


## Contents
![Python](https://img.shields.io/badge/python-v3.6+-blue.svg)
![Dependencies](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)

- [Movie Recommendation System Overview](#movie-recommendation-system-overview)
   - [Simple Recommender](#simple-recommender)
   - [Content-Based Recommender](#content-based-recommender)
   - [Collaborative Filtering using SVD](#collaborative-filtering-using-svd)
   - [Hybrid Recommender](#hybrid-recommender-system)
   - [Common Challenges](#common-challenges)
   
 - [About DataSet](#about-dataset-used)

## Movie Recommendation System Overview

The Movie Recommendation System is a comprehensive platform designed to assist users in discovering new movies tailored to their individual preferences. Leveraging cutting-edge machine learning algorithms and natural language processing techniques, the system offers a range of recommendation strategies to enhance the movie discovery process.

These strategies include Simple Recommenders, which provide general movie suggestions based on popularity and genre, as well as Content-Based Recommenders that analyze movie descriptions and metadata. Additionally, Collaborative Filtering techniques using Singular Value Decomposition (SVD) are employed to understand user preferences and generate accurate predictions of movie ratings. The system's Hybrid Recommender combines the strengths of content-based and collaborative filtering approaches to deliver diverse and engaging recommendations. 

Continuously evolving based on user feedback and data-driven insights, the Movie Recommendation System aims to provide users with a seamless and personalized movie discovery experience.

#### Simple Recommender
The Simple Recommender provides generalized recommendations based on movie popularity and genre, furnishing users with top-rated movies across various genres. By implementing an IMDB weighted rating method, movies are ranked according to their popularity and critical acclaim, ensuring high-quality recommendations. This model serves as a baseline for comparison with more advanced recommendation techniques.

#### Content-Based Recommender
The Content-Based Recommender utilizes two types of content-based recommendation techniques:

Movie Description Based Recommender: This technique uses movie descriptions, taglines, and metadata such as cast, crew, genre, and keywords to suggest similar movies to users based on their preferences. Through TF-IDF vectorization and cosine similarity, this recommender generates tailored recommendations aligned with the user's interests and viewing history.

Metadata Based Recommender: In addition to movie descriptions, this recommender incorporates metadata such as cast, crew, genre, and keywords to enhance recommendation accuracy by comprehensively considering movie attributes. By analyzing textual and categorical features of movies, this recommender ensures that recommendations are relevant and diverse.

#### Collaborative Filtering using SVD
Collaborative Filtering enables personalized recommendations by analyzing user-item interactions and identifying similar users to estimate a user's preferences. Leveraging the Surprise library and Singular Value Decomposition (SVD), this recommender provides precise predictions of user ratings and suggests movies that align with the user's tastes. By training on user ratings and movie metadata, the system enhances recommendation quality and user satisfaction.

#### Hybrid recommender system
The Hybrid Recommender integrates techniques from content-based and collaborative filtering engines to deliver more personalized and diverse recommendations. By incorporating both user preferences and movie attributes, this hybrid model offers a unique and tailored movie-watching experience for each user. Through a combination of machine learning algorithms and user-item interactions, the system ensures that recommendations are relevant and engaging.

#### Common Challenges
Throughout the development of this project, various challenges were encountered, including:

Data Sparsity: Dealing with sparse user-item interaction matrices and limited user ratings for some movies.
Cold Start Problem: Addressing the cold start problem for new users and new movies without sufficient data for accurate recommendations.
Scalability: Ensuring that recommendation algorithms scale efficiently to handle large datasets and provide real-time recommendations.
Evaluation Metrics: Selecting appropriate evaluation metrics to assess the performance and effectiveness of recommendation models accurately.

## About Dataset used

Context

These files contain metadata for all 45,000 movies listed in the Full MovieLens Dataset. The dataset consists of movies released on or before July 2017. Data points include cast, crew, plot keywords, budget, revenue, posters, release dates, languages, production companies, countries, TMDB vote counts and vote averages.

This dataset also has files containing 26 million ratings from 270,000 users for all 45,000 movies. Ratings are on a scale of 1-5 and have been obtained from the official GroupLens website.

Content

This dataset consists of the following files:

movies_metadata.csv: The main Movies Metadata file. Contains information on 45,000 movies featured in the Full MovieLens dataset. Features include posters, backdrops, budget, revenue, release dates, languages, production countries and companies.

keywords.csv: Contains the movie plot keywords for our MovieLens movies. Available in the form of a stringified JSON Object.

credits.csv: Consists of Cast and Crew Information for all our movies. Available in the form of a stringified JSON Object.

links.csv: The file that contains the TMDB and IMDB IDs of all the movies featured in the Full MovieLens dataset.

links_small.csv: Contains the TMDB and IMDB IDs of a small subset of 9,000 movies of the Full Dataset.

ratings_small.csv: The subset of 100,000 ratings from 700 users on 9,000 movies.

The Full MovieLens Dataset consisting of 26 million ratings and 750,000 tag applications from 270,000 users on all the 45,000 movies in this dataset can be accessed [here](https://grouplens.org/datasets/movielens/latest/)

Acknowledgements

This dataset is an ensemble of data collected from TMDB and GroupLens.
The Movie Details, Credits and Keywords have been collected from the TMDB Open API. This product uses the TMDb API but is not endorsed or certified by TMDb. Their API also provides access to data on many additional movies, actors and actresses, crew members, and TV shows. You can try it for yourself [here](https://www.themoviedb.org/documentation/api).

The Movie Links and Ratings have been obtained from the Official GroupLens website. The files are a part of the dataset available [here](https://grouplens.org/datasets/movielens/latest/)

Contributions and feedback are welcome to further enhance the functionality and performance of the recommendation system.

Note: This project is available under the MIT License, enabling collaboration and contributions from the community to enhance and expand the capabilities of the movie recommendation system.

 

# Movie Recommendation System using TMDB Dataset

## Overview
This project builds a movie recommendation system using the TMDB (The Movie Database) dataset. The system recommends movies based on similarity in genres, keywords, cast, crew, and overview.

It uses content-based filtering to suggest movies similar to a given input.

## Dataset

Dataset Source:  
https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata/data

The dataset contains metadata for thousands of movies including:
- Titles and overviews  
- Genres and keywords  
- Cast and crew details  
- Budget and revenue  
- Popularity and ratings  

Files used:
- tmdb_5000_movies.csv
- tmdb_5000_credits.csv

## Project Workflow

1. Data Collection  
   - Load movies and credits datasets  
   - Merge both datasets  

2. Data Preprocessing  
   - Handle missing values  
   - Select important columns  
   - Convert JSON columns into readable format  

3. Feature Engineering  
   - Extract genres, keywords, cast, and director  
   - Combine features into a single "tags" column  

4. Text Processing  
   - Convert text to lowercase  
   - Remove spaces and noise  

5. Vectorization  
   - Use CountVectorizer  
   - Remove stopwords  
   - Convert text into vectors  

6. Similarity Calculation  
   - Apply cosine similarity  

7. Recommendation System  
   - Input: movie name  
   - Output: top 5 similar movies  

## Technologies Used

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- NLTK  

## Usage

Run Jupyter Notebook:
jupyter notebook

Example:
recommend("Avatar")

## Key Concept

The system uses cosine similarity to recommend movies based on content similarity.

## Future Improvements

- Add collaborative filtering  
- Deploy using Streamlit  
- Improve NLP techniques  
- Add user personalization  

## Author

Charan Teja Goud

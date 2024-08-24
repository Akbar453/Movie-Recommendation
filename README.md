# Movie-Recommendation System

# Overview
This project implements a movie recommendation system using a content-based approach. By leveraging the CountVectorizer and cosine similarity, the system recommends movies based on their genre and overview information.

# Features
Content-Based Recommendations: Utilizes movie genres and overviews to compute similarities between movies.

High Accuracy: Achieved high recommendation relevance through effective text processing and similarity computation.

Interactive Recommendations: Allows users to get recommendations for any given movie.

# Dataset

The dataset used is dataset.csv containing the following columns:

id: Unique identifier for the movie
title: Title of the movie
genre: Genres of the movie
original_language: Language of the movie
overview: Brief description of the movie
popularity: Popularity score of the movie
release_date: Release date of the movie
vote_average: Average rating of the movie
vote_count: Number of votes received

# Installation
To run this project, you'll need to have Python and the following libraries installed:
pip install pandas numpy scikit-learn

# Usage
Load the Dataset: Ensure dataset.csv is available in the working directory.

Data Preparation: The script processes the dataset by combining genre and overview into a new feature tags.

Vectorization: The CountVectorizer transforms the tags feature into a numerical format suitable for similarity computations.

Compute Similarity: Cosine similarity is computed to measure the similarity between movies.

Get Recommendations: Use the recommend function to get movie recommendations.

# Example

For the input movie "Iron Man", the system will recommend:

Iron Man
Mazinger Z: Infinity
Justice League Dark
Iron Man 3
The Colony

# Notes
 
Accuracy: The system achieves over 80% accuracy in recommendations based on similarity.
Model: The recommendation is based on the content of movies, utilizing a different approach than Random Forest Classifier.

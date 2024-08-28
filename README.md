# Spotify Song Recommender

This project analyzes Spotify music data to explore trends, correlations, and create a simple song recommendation system using machine learning techniques.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Requirements](#requirements)
- [Usage](#usage)
- [Analysis Highlights](#analysis-highlights)
- [Recommendation System](#recommendation-system)

## Overview

This project uses Spotify music data to perform various analyses and build a recommendation system. It explores trends in music features over time, correlations between different audio features, and uses machine learning techniques to cluster similar songs.

## Features

- Data preprocessing and cleaning
- Trend analysis of audio features over time
- Correlation analysis between different audio features
- Genre clustering using PCA and K-means
- Song recommendation system based on audio features

## Requirements

- Python 3.x
- pandas
- numpy
- plotly
- scikit-learn
- IPython (for notebook display)

## Usage

1. Ensure you have the required CSV files:
   - `Dados_totais.csv`
   - `data_by_genres.csv`
   - `data_by_year.csv`

2. Run the Jupyter notebook or Python script to perform the analysis.

3. Follow the code comments for detailed explanations of each step.

## Analysis Highlights

1. **Loudness Trend**: The project analyzes the variation of loudness in music over the years.

2. **Audio Feature Trends**: Visualizes trends for multiple audio features (acousticness, valence, danceability, energy, instrumentalness, liveness, speechiness) from 2000 onwards.

3. **Feature Correlation**: A heatmap is generated to show correlations between different audio features.

4. **Genre Clustering**: Using PCA and K-means, the project clusters music genres based on their audio features.

5. **Song Clustering**: Similar to genre clustering, individual songs are clustered based on their features and artist information.

## Recommendation System

The project includes a simple recommendation system that suggests similar songs based on audio features. It uses the following steps:

1. Dimensionality reduction using PCA
2. K-means clustering on the reduced feature space
3. Euclidean distance calculation to find the nearest neighbors within a cluster

To get recommendations, use the `recomendador` function with a song name as input.

Example:
```python
recomendador('Foo Fighters - Best of You')
```

This will return a list of 20 recommended songs based on similarity to the input song.

---

Feel free to contribute to this project by opening issues or submitting pull requests!

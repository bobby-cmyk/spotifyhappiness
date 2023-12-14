Measuring happiness with Spotify's listening history
https://medium.com/@aikenonght/how-happy-areyou-93de90de6638

# Spotify Data Analysis and Visualization
## Overview
This Python script is designed to analyze and visualize Spotify playlist data, focusing on the positiveness of personal and global top tracks from 2016 to 2022. It leverages the Spotify Web API to fetch track details and audio features, and uses Plotly for creating interactive visualizations.

## Dependencies
* pandas: For data manipulation and analysis.
* spotipy: For interacting with the Spotify Web API.
* os: For environment variable management.
* dotenv: For loading environment variables from a .env file.
* plotly: For creating interactive charts.
* numpy: For numerical computations.
* chart_studio: For publishing charts to Chart Studio.

## Script Features
* API Authentication:
  * Authenticates with Spotify API and Chart Studio using credentials stored in environment variables.
* Data Collection:
  * Fetches tracks from personal and global Spotify playlists for each year from 2016 to 2022.
  * Extracts audio features for each track using the Spotify API.
* Data Transformation:
  * Transforms data for visualization, focusing on the 'valence' feature to measure positiveness.
* Data Visualization:
  * Creates ridgeline plots to show the distribution of positiveness in personal and global playlists over the years.
  * Compares median valence (positiveness) of personal tracks against global top tracks for each year in a line chart.
* Chart Studio Integration:
  * Uploads the generated plots to Chart Studio for sharing and embedding purposes.

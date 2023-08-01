# GNOD - Song Recommendation

## Introduction
Welcome to the "GNOD - Song Recommendation" project repository. This project aims to provide song recommendations to users based on their input songs' audio features. The recommendation system uses clustering and comparative analysis techniques to identify songs with similar characteristics. The repository contains the code for data retrieval, data analysis, clustering, and the song recommendation functionality.

## Files in the Repository
GNOD Project.ipynb: A Jupyter Notebook containing the main project code. It includes all three parts of the project, i.e., data retrieval, data analysis, and song recommendation.
Get_Songs_From_Playlists.ipynb: A Jupyter Notebook with the code responsible for retrieving songs from Spotify playlists and gathering audio features for analysis.
KMeans.plk: A pre-trained KMeans clustering model saved as a pickle file. This model is used to cluster songs based on their audio features.
lab-unsupervised-learning-intro.ipynb: A Jupyter Notebook introducing unsupervised learning concepts and showcasing the application of KMeans clustering to analyze audio features.
Top_100_Billboard.csv: A CSV file containing data from the "Top 100 Billboard" songs. This dataset was obtained through web scraping from the Billboard website.
final_clean_df.csv: A CSV file containing the final cleaned DataFrame, which includes audio features, song names, and cluster assignments for the songs.
numerical.csv: A CSV file containing the numerical data used for clustering and analysis.
playlist_2.csv: A CSV file containing the playlist data, including song IDs, song names, and artist names.
playlist_audio.csv: A CSV file containing the audio features extracted from Spotify for the songs in the playlist.
readme.md 2: A readme file from a previous version of the project.
scaler_sd.pkl: A pre-trained scaler used to standardize the numerical data before clustering.

## Code Overview
### Data Retrieval (Get_Songs_From_Playlists.ipynb):

- Utilizes the Spotify Web API to retrieve songs from specified playlists.
- Collects audio features for the retrieved songs.
- Creates a DataFrame with the audio features and song details.
- Saves the playlist data and audio features to CSV files.
  
### Data Analysis and Clustering (lab-unsupervised-learning-intro.ipynb):

- Reads the playlist data and audio features CSV files.
- Performs data preprocessing and standardization on the numerical data.
- Introduces unsupervised learning concepts and the application of KMeans clustering to analyze audio features in "lab-unsupervised-learning-intro.ipynb".
- Uses the KMeans clustering algorithm to cluster the songs based on their audio features.
- Determines the optimal number of clusters using the elbow method and silhouette score.
- Saves the pre-trained KMeans model and scaler as pickle files.
  
### Song Recommendation (GNOD Project.ipynb):

- Allows the user to input a song.
- Checks if the input song is in the "Top 100 Billboard."
- If not, retrieves audio features for the input song and assigns it to a cluster using the pre-trained model and scaler.
- Recommends a random song from the same cluster as the input song, if available.
  
## Conclusion
The "GNOD - Song Recommendation" project provides a song recommendation system that allows users to discover new songs based on their preferences. It utilizes Spotify's audio features and clustering techniques to group similar songs together. The repository includes code for data retrieval, analysis, and recommendation, as well as pre-trained models and data files for seamless execution. Feel free to explore the code, datasets, and recommendations to enhance your music discovery experience. Your feedback and contributions are welcome as we continue to refine and expand this project. Enjoy exploring and listening to new music!






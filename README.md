# Recommendation-for-Artist-to-Improve-Popularity-on-Spotify-
## The problem that motivates the analysis you will conduct
Sometimes Spotify users want to search for artists similar to whom the user is currently listening to. We know that Spotify has a recommendation function based on music genres. Therefore, we are wondering if music artists can be segmented into liked groups based on their music forms and style. Once artists are classified, Spotify will be able to pull artist names from the same cluster which the currently listened artist is in. By adding the feature of recommending similar artists, Spotify’s usability will improve as well. 
## Dataset
Source: https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks?select=data.csv
Dataset name:
Spotify “Data_by_Artist.csv” Dataset

This dataset contains 32,539 unique artists between the year of 1921 and 2021 collected from Spotify Web API. The rows represent different artists, and columns represent different audio features.

Attributes (columns in the dataset) we are planning to focus on:
- artists: artist name
- acousticness (Ranges from 0 to 1): describes how acoustic a song is. A score of 1.0 means the song is most likely to be an acoustic one.
- danceability (Ranges from 0 to 1): describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable
- duration_ms (Integer typically ranging from 200k to 300k): duration in milliseconds.
- energy (Ranges from 0 to 1): represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy
- instrumentalness (Ranges from 0 to 1): represents the amount of vocals in the song. The closer it is to 1.0, the more instrumental the song is.
- liveness (Ranges from 0 to 1): the relative duration of the track sounding as a live performance.
- loudness (Float typically ranging from -60 to 0): the relative loudness.
- tempo (Float typically ranging from 50 to 150): the speed of the track.
- speechiness (Ranges from 0 to 1): the relative length of the track containing any kind of human voice

## Your proposed analysis methodology
We plan to use the learning obtained from the class such as kmeans, PCA and other clustering techniques that we will be learning in the next several sessions to conduct the analysis.

PCA can be utilized to do dimensional reduction. Some features in our dataset might have high correlations, thus, applying PCA will help us reduce some noise from the dataset. In use of PCA, we expect to retain an overall explained variance of our dataset at 95%; therefore, principal components will have a high summarization value. After PCA, we can further use cluster analysis techniques such as KMeans to segment the data points.


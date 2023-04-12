# Introduction

This repository contains my capstone group project at UCLA's PIC16A (Python with Applications) class. This class covers various libraries such as **Numpy, Seaborn, Matplotlib and Pandas**. It also explores Machine Learning algorithms such as **K-nearest neighbors (KNN), Linear Regression, and Random Forest models**.

# Motivation
Traditionally, this class uses the [Palmer Penguins](https://philchodrow.github.io/PIC16A/content/IO_and_modules/IO/palmer_penguins.csv) data. However, our group believed that this dataset was too limited in terms of datapoints (400) and was nicely clustered for the purposes for this class. We sought to challenge our data analysis and Python skills by working on *messy real-life datasets*.

Therefore, our group explored various sources and came across [Kaggle's Spotify dataset](https://www.kaggle.com/datasets/sashankpillai/spotify-top-200-charts-20202021) describing all songs which made it to Spotify's Top 200 Charts in 2020-2021. This dataset stood out to us because ==**we were curious to see if we could utilize the machine learning algorithms we've learnt so far to predict something as subjective as song taste**== (which introduces a large amount of unpredictability and randomness into our dataset).

# Description of Dataset
| Field                      | Description                                                                                                                          |
| --------------------------| ------------------------------------------------------------------------------------------------------------------------------------ |
| Highest Charting Position  | The highest position that the song has been on in the Spotify Top 200 Weekly Global Charts in 2020 & 2021.                           |
| Number of Times Charted    | The number of times that the song has been on in the Spotify Top 200 Weekly Global Charts in 2020 & 2021.                             |
| Week of Highest Charting   | The week when the song had the Highest Position in the Spotify Top 200 Weekly Global Charts in 2020 & 2021.                           |
| Song Name                  | Name of the song that has been on in the Spotify Top 200 Weekly Global Charts in 2020 & 2021.                                        |
| Song iD                    | The song ID provided by Spotify (unique to each song).                                                                               |
| Streams                    | Approximate number of streams the song has.                                                                                           |
| Artist                     | The main artist/ artists involved in making the song.                                                                                 |
| Artist Followers           | The number of followers the main artist has on Spotify.                                                                               |
| Genre                      | The genres the song belongs to.                                                                                                      |
| Release Date               | The initial date that the song was released.                                                                                          |
| Weeks Charted              | The weeks that the song has been on in the Spotify Top 200 Weekly Global Charts in 2020 & 2021.                                     |
| Popularity                 | The popularity of the track. The value will be between 0 and 100, with 100 being the most popular.                                     |
| Danceability               | Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable. |
| Acousticness               | A measure from 0.0 to 1.0 of whether the track is acoustic.                                                                            |
| Energy                     | Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy.                                           |
| Instrumentalness           | Predicts whether a track contains no vocals. The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content.                                             |
| Liveness                   | Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live.                                                   |
| Loudness                   | The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track. Values typical range between -60 and 0 db.                                                  |
| Speechiness                | Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value.         |
| Tempo                      | The overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration.    |
| Valence                    | A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry). |
| Chord                      | The main chord of the song instrumental.                                                                                            |

# Main Files
- [spotify_dataset.csv](https://github.com/jia-shing/pic16a-spotify/blob/main/spotify_dataset.csv): Dataset exported from Kaggle
- [Spotify_EDA_v4.ipynb](https://github.com/jia-shing/pic16a-spotify/blob/main/Spotify_EDA_v4.ipynb): Data cleaning, data mapping, EDA and ML pipeline are all consolidated in one Jupyter Notebook file
- [Spotify_EDA_v4.pdf](https://github.com/jia-shing/pic16a-spotify/blob/main/Spotify_EDA_v4.pdf): Jupyter Notebook exported as PDF via LaTeX
- Other .csv files are for mapping and their respective use cases are described in the ipynb and PDF files

# Critique
Due to the timeline of this project, we consulted with the instructor of this course and decided to narrow down each song such that it maps to exactly one (of the five) genre. This may help with decision region plotting and reduce the complexity of our models. However, to do so, we had to manually narrow down each song into one genre. Even though we tried to reduce subjectivity and avoid introducing more randomness into our dataset by assigning one team member to carry out all the mapping, we think that this may not be the best way to proceed.

# Suggestion
Classify the songs based on quantitative variables of the song such as Valence, Tempo, Danceability etc. This may be a much more objective way of doing things. However, this may also mean that we introduce mutlicollinearity into the dataset since Genre is directly correlated to a handful of quantitative variables in the dataset.

# Contributions
This group project wouldn't have been possible without the support of my teammates LiYuan Tan and Sidney Shah. I truly appreciate their wilingness to explore something other than a well-trodden path and I think it speaks to their character.


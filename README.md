# Spotify-YouTube Exploratory Data Analysis
The project was aimed at looking at the correlation between attributes that would contribute to an increase in the number of views on YouTube, streams on Spotify and
comments. Main focus was on danceability and energy attributes.

# Prerequisites
.Python
.Jupyter Notebook
.Python Libraries(pandas, numpy, matplotlib, seaborn)

# Data Source
The data was downloaded from Kaggle, link:https://www.kaggle.com/datasets/salvatorerastelli/spotify-and-youtube

# Data Preprocessing
.Removed the Unnamed column after creating a copy of the data, Converted data in the Artist, Track, Album, Title and Channel columns to begin with capital letters for uniformity
.Dropped some columns not needed for analysis ('Url_spotify', 'Uri', 'Url_youtube', 'Title', 'Description')
.For missing values (Ones in Likes column were filled with the mean from the column), (Ones in Comments column were filled with mean based on the album type),
(Ones in Stream column were filled with mean based on whether the video was official or not)
.Outliers were removed from the column(Duration) based on quantile
.Danceability and Energy classified and their relationship observed.

# Exploratory Data Analysis
Mainly used visualizations were histograms and scatterplots plus a heatmap. Music with higher energy(0.3 - 1.0) had a relatively higher views and stream rates compared to
lower energy music. On the general this relationship was true for danceability too though in some cases vice versa was true.

# Exploratory Data Analysis on Spotify Popular Tracks of 2023

## Introduction 
This project explores a dataset of popular Spotify tracks in 2023. The project aims to analyze trends and insights into music popularity, genres, and other characteristics. We have the following questions to ponder:
- Which genres, tracks, and artists are most popular?
- What features contribute to a track's popularity?

## Dataset Overview 

We start by loading the libraries that are to be used in the program. We will be utilizing pandas for easier handling of data, matplotlib for the data visualization, and seaborn to enhance the capabilities of data visualization (matplotlib).

import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

Then we load the dataset:

import zipfile
with zipfile.ZipFile('top-spotify-songs-2023.zip', 'r') as zip_ref: zip_ref.extractall('spotify_data')

df = pd.read_csv('spotify_data/spotify-2023.csv', encoding = 'latin1')
print('Shape of the dataset: ', df.shape)

Then display the first few rows:

df.head()

Afterwards, we load the basic information about the dataset:

df.info() 


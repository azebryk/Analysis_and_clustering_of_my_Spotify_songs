# Analysis and Clustring of My Favorite Spotify Songs: Project Overview


I am huge music fan and, in my opinion, there is no obvious pattern what types of songs I like. Therefore, I decided to look  a little bit deeper into it, perform analysis and try to distinguish some groups.

The aim of this project is to analyze and cluster my favorite Spotify songs. This project consist following steps:
* Data gathering 
* Data preparation and exploratory analysis of my streaming history.
* Spotify API: Adjsuting class from https://github.com/codingforentrepreneurs/. Adding extra methods for my case. 
* K-Means clustering. Finding accurate numer of clusters using elbow method.
* Cluster visualisation using TSNE.


## Technologies Used:

*	Python version 3.8.3
*	Pandas
*	Numpy
*	Matplotlib
*	Seaborn 
* Spotify API
*	JSON
*	Requests
*	urlib.parse
* base64
* K-means clustering
* TSNE


## Data Sources and Preparation:
1.  My streaming history 
I reequested songs, which I listned to during last 365 days  from Spotify website. Then I kept only songs, which was played more than 5 times.
2. Spotify API
I used it to get details about each song, audio features like danceability, loudness or tempo.
For this I used code from https://github.com/codingforentrepreneurs/
I modified this code and added methods to the class aproperate to my case.



## EDA
I looked at the general info and distributions of the data. Here are some highlights:
### Distribution of danceability
<p align="center">
  <img src="https://github.com/azebryk/Analysis_and_clustering_of_my_Spotify_songs/blob/master/images/danceability.JPG" width=800>
</p>
<p align="center">
  <img src="https://github.com/azebryk/Analysis_and_clustering_of_my_Spotify_songs/blob/master/images/tempo_dance_key.JPG" width=800>
</p>

## K-Means clustering
Selecting number of clusters using elbow method:
<p align="center">
  <img src="https://github.com/azebryk/Analysis_and_clustering_of_my_Spotify_songs/blob/master/images/elbow.JPG" width=800>
</p>

## Cluster visualisation using TSNE.
Visualisation of 7 clusters using TSNE:
<p align="center">
  <img src="https://github.com/azebryk/Analysis_and_clustering_of_my_Spotify_songs/blob/master/images/t_sne.JPG" width=800>
</p>

#### Comment/Observation:

- Note: 2021 curve is highlighted
- PM2.5 lvl is significantly lower during firts week and in general rather lower than in previous years
- missing days can be observed (2019, 2017)
- 2015 was omitted due to bad quality of data
  
To confirm our observation let's check average temperature and average PM2.5 level in April for each year.

<p align="center">
  <img src="https://github.com/azebryk/Analysis_and_clustering_of_my_Spotify_songs/blob/master/images/t_sne.JPG" width=700>
</p>



## Code and Resources Used 
**Python Version:** 3.8.3  
**Packages:** pandas, numpy, sklearn, matplotlib, seaborn, requests, BeautifulSoup

**Spotify API, Source:** https://github.com/codingforentrepreneurs/


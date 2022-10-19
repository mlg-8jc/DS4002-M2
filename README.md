# DS 4001 M2
---

## Table of contents[![](./images/pin.svg)](#table-of-contents)
1. [INTRODUCTION](#introduction)
2. [HYPOTHESIS](#hypothesis)
3. [SRC](#src)
4. [DATA](#data)
5. [FIGURES](#figures)
6. [REFERENCES](#references)

---

## INTRODUCTION[![](./images/pin.svg)](#introduction)

Everyone listens to music, but everybody’s tastes are different. However, there appears to be similarities between songs that become popular. There seems to be similarities in rhythms, beats per minute, and other characteristics of these songs [1]. We would like to dive deeper into what truly makes a Top 100 song by running analyses on certain characteristics in each song. 

In “What Makes a Song Likable”, Ashrith analyzed what factors contribute to the popularity of songs and conducted research on “Top Spotify Tracks of 2017”, a data set on Kaggle. By his scatterplot of the Audio Features parameters, he found that danceability, energy and valence are strongly correlated with the popularity of a song. Danceability explains how suitable a track is for dancing and is measured from 0 to 100. Energy is a measure of intensity and activity. Typically, energetic music is fast and loud. These two variables will increase the chance of being in the Top 50 Spotify songs. Inspired by the result, we would like to investigate if these trends have changed over the past five years. [2]


---

## HYPOTHESIS[![](./images/pin.svg)](#hypothesis)

**Within the audio features of each song on Spotify, the variables danceability and valence are correlated to the current top 100 most popular songs on Spotify, as a song appearing on the Top 100 chart has a greater likelihood of having a score of 0.5 for danceability, and 0.5 for valence, than having a score below 0.5 for those two variables.**

---

## SRC[![](./images/pin.svg)](#src)
![made-with-R](https://img.shields.io/badge/Made%20with-R-1f425f.svg)<br>

### Installing/Building Code

First, one must make sure that R and RStudio are installed on their system. Then, you can download the script from our src folder, along with the dataset in the data folder. Make sure that the files are saved into the same directory and change the working directory to where the files are located. 

### Spotity API in R
`spotifyr` is required to access spotify API. It is an R wrapper for pulling audio features and all the information from Spotify's API in bulk. In order to utilize the Spotify API in R, one must install the spotifyr package by running "install.packages('spotifyr)". Then, the spotifyr package needs to be called in the beginning of the R file by running "library(spotifyr)". To get the information from Spotify, one must have authorzation tokens (both client ID and client secret). To do that, one can create a Spotify Developer account and find all the required information on the Dashboard page.

### Usage of Code

One would want to use our code to replicate and verify our results, or to possibly run further analysis on our dataset.


---
## DATA[![](./images/pin.svg)](#data)
For full data, please click [here]()

For the data dictionary, please click [here](./data/Data_Dictionary)

The first six rows of our data set are shown below...



---

## FIGURES![](./images/pin.svg)

### **Figures Table**
* Valence and Popularity


### **Valence and Popularity**
![](./figures/Graph_Valence_and_Popularity.png)



---

## REFERENCES

[1]S. Middler, “Is There a Formula to Making a Popular Song?,” Information Expositions F2019, Sep. 16, 2019. https://medium.com/information-expositions-f2019/is-there-a-formula-to-making-a-popular-song-c503530cd729 (accessed Oct. 05, 2022).
‌
[2] Ashrith, “What Makes a Song Likable,” Towards Data Science, Dec. 3, 2018. https://towardsdatascience.com/what-makes-a-song-likeable-dbfdb7abe404
[3].“Web API Reference: Spotify for Developers.” Home, https://developer.spotify.com/documentation/web-api/reference/#/operations/get-recommendations. 


### OTHER LINKS

- Access our MI1 assignment from [here](https://collab.its.virginia.edu/access/content/attachment/856376d0-e4da-47eb-9375-a797b1752c6f/Assignments/9e9b7b2b-222c-49b7-9cdf-ab961fabc74c/M1-2%20Establish%20Data%20to%20Analysis%20Plan%20_1_.pdf) 👋
- Access our MI2 assignment from [here](https://collab.its.virginia.edu/access/content/attachment/856376d0-e4da-47eb-9375-a797b1752c6f/Assignments/3cec6e30-17b0-4b8b-9e66-2a74e88cf55b/M2-2%20Group%206.pdf) 🤝

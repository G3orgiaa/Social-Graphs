## Introduction

For this's year project we have chosen to analyze the Viking Series dataset. As a little bit of history first, Vikings is a historical television drama series, that was first aired in Canada in 2013. Inspired by true events and characters, the shows tells the story of Ragnar Lothbrok, one of the best-known legendary Norse heroes and notorious as the scourge of England and France (source Wikipedia).

We decided to choose the Vikings show as our dataset for many reasons. First of all it's an award winning amazing show! Second of all, we are living in Denmark, the  country of origin of vikings. Third, the dataset itself provide plenty analysis opportunities, between all the show's elements. Last but not least, the game Assasins Creed: Valhalla just recently was launched so, if you are a gamer the vikings topic is more relevant than ever ;).

The ambition of this notebook and site, is to give a basic but clear analysis on the viking's tv show's elements to someone who is not an expert in network analysis or python.

## A smal description of the dataset

We used the Fandom Wiki page for downloading the relevant data. All the files that were used during the analysis can be found here (https://drive.google.com/drive/folders/1j7NCzDaNx_NBu0T2vC4U2qIWAUTkWVV8?usp=sharing). For the views dataset, data from the internet were used. For more information on the data, please refer to the python notebook.

## Network and Text Analysis
First of all we conducted some preliminary analysis of the data. Using API and python, the show's element (characters, episodes and seasons) were extracted, and stored in separate files. Before that, elements that were leading to blank wiki pages had to be elimate from the dataset while non ascii characters had to be transformed into a proper unicode format.

Apart from the files for every element, two separate files were created; one for storing the characters that died during each season and a second one for keeping the main and recurring cast of each season.

With the network package called netoworkx, an undirected graph was created, storing all show's elements. The graph consists of 10700 edges and 603 nodes. 







### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for



**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

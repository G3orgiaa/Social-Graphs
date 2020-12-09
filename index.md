## Introduction

For this's year project we have chosen to analyze the Viking Series dataset. As a little bit of history first, Vikings is a historical television drama series, that was first aired in Canada in 2013. Inspired by true events and characters, the shows tells the story of Ragnar Lothbrok, one of the best-known legendary Norse heroes and notorious as the scourge of England and France (source Wikipedia).

We decided to choose the Vikings show as our dataset for many reasons. First of all it's an award winning amazing show! Second of all, we are living in Denmark, the  country of origin of vikings. Third, the dataset itself provide plenty analysis opportunities, between all the show's elements. Last but not least, the game Assasins Creed: Valhalla just recently was launched so, if you are a gamer the vikings topic is more relevant than ever ;).

The ambition of this notebook and site, is to give a basic but clear analysis on the viking's tv show's elements to someone who is not an expert in network analysis or python.

## A smal description of the dataset

We used the Fandom Wiki page for downloading the relevant data. All the files that were used during the analysis can be found here (https://drive.google.com/drive/folders/1j7NCzDaNx_NBu0T2vC4U2qIWAUTkWVV8?usp=sharing). For the views dataset, data from the internet were used. For more information on the data, please refer to the python notebook.

## Network and Text Analysis
First of all we conducted some preliminary analysis of the data. Using API and python, the show's element (characters, episodes and seasons) were extracted, and stored in separate files. Before that, elements that were leading to blank wiki pages had to be elimate from the dataset while non ascii characters had to be transformed into a proper unicode format.

Apart from the files for every element, two separate files were created; one for storing the characters that died during each season and a second one for keeping the main and recurring cast of each season.

With the network package called netoworkx, an undirected graph was created, storing all show's elements. The graph consists of 10700 edges and 603 nodes. Then  chose the propose centrality measurement in order to identify the most significan nodes of the graphs. The top 15 most important nodes are:

('Vik', 420)
('Vikings', 381)
('Ragnar', 285)
('Bjorn', 232)
('Kattegat', 225)
('Lagertha', 220)
('Harald', 201)
('Ivar', 191)
('Ubbe', 179)
('Rollo', 172)
('Floki', 171)
('Season 5', 168)
('Hvitserk', 167)
('Earl', 165).

Next, we tried to answer some questions. First of all, which, out of the 6 total seasons is the most popular?. We found out that the most popular season is the season 1 and the least popular is seaosn 6. Moreover, we noticed that, there is an almost steady reduction in the number of views season by season. This is why, the next question was generated. What is the impact that may has on the show's views, the lead's actors death? We chose the three most significant characters (Ragnar, Bjorn and Lagertha) and firstly we checked their life status. Thw way to go about this was to check whether their name(string) was part of the files that contained each's season's deaths. We found out that out of the three, only Ragnar, has died so the next step was to find out when. He died during season 4. Looking at the graphs, we noticed that after his death, the was an extra reduction at the show's ratings. Our last question was in relation to the show's critic's ratings and vierships'. More specifically, the questions is: do bad viership's mean bad rating's as well? To our suprise, the answer is no. For instance, season 3 and 6 have the highest ratings in Rotten Tomatoes but are amongst the seasons with the lowers numbers in views.

## Link to Notebook

For more information please refere here https://nbviewer.jupyter.org/github/G3orgiaa/Social-Graphs/blob/gh-pages/Project%20B.ipynb

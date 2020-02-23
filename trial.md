---
title: "Allison's Portfolio"
output: 
  flexdashboard::flex_dashboard:
    orientation: rows
    vertical_layout: fill
    storyboard: true
    theme: cerulean
---

```{r setup, include=FALSE}
library(flexdashboard)
library(tidyverse)
library(spotifyr)
library(knitr)
library(DT)
library(datasets)
library(plotly)
```

Initial Data and Observations
========================================

Column {data-height=400}
-----------------------------------------------------------------------

### An inquiry into the structure of an album and how it may have changed over time.

```{r}

```


I have chosen to focus on the discography of one of my personal favorite bands, Twenty One Pilots. I am interested in Twenty One Pilots' albums specfically as they have been deemed 'concept albums' with distinct, yet somewhat interconnected, storylines and themes. With this in mind, I would be interested in investigating whether or not these themes are solely recognizable in the media content associated with the albums *(such as music videos and linked websites)*, or in the attributes and structures of the albums themselves.
I also chose to focus on the music of Twenty One Pilots as the band has been making music for over a decade and I am intrigued by the potential evolution of the band's albums throughout their career. 


Column {data-height=600}
-----------------------------------------------------------------------

### Have certain aspects of Twenty One Pilots' music changed between albums?

```{r}

```
Twenty One Pilots' discography *(that which is available on Spotify)* is made up of four albums, 54 songs, which have been released between 2009 and 2018. I chose to first analyze the mean values, along with their corresponding standard deviations, of selected categories provided by Spotify's data and compare them between the four albums. I organized these data points into a table *(shown below)*.


| Attributes | | Twenty One Pilots (2009) | Vessel (2013) | Blurryface (2015) | Trench (2018) |
| :--------- |:-- | :----------------------: | :-----------: | :---------------: | :-----------: |
| **Danceability** | `Mean` | 0.57 | 0.68 | 0.64 | 0.67 |
|  | `Standard Deviation` | 0.15 | 0.12 | 0.09 | 0.08 |
| **Energy** | `Mean` | 0.54 | 0.62 | 0.73 | 0.62 |
|  | `Standard Deviation` | 0.21 | 0.24 | 0.12 | 0.14 |
| **Loudness** | `Mean` | -7.78 | -6.35 | -5.59 | -7.57 |
|  | `Standard Deviation` | 2.11 | 2.86 | 0.95 | 1.61 |
| **Liveness** | `Mean` | 0.15 | 0.14 | 0.16 | 0.19 |
|  | `Standard Deviation` | 0.08 | 0.06 | 0.12 | 0.12 |
| **Valence** | `Mean` | 0.31 | 0.56 | 0.54 | 0.44 |
|  | `Standard Deviation` | 0.17 | 0.20 | 0.17 | 0.18 |
| **Tempo** | `Mean` | 123 | 126 | 122 | 115 |
|  | `Standard Deviation` | 23.5 | 24.9 | 28.0 | 23.6 |

Upon first glance, it seems as though the band has created fairly consistent content with each of their four albums. If anything, they may have exhibited a kind of curve in regards to some aspects, such as *loudness* and *valence*, in which they had deviated from their original style but have since tried to return to it. I plab to further review this in the **Vizualizations** section.

### Is there a pattern to the structure of Twenty One Pilots' albums?

```{r}

```
Through a comparative analysis of the four albums, I plan to study the potential method by which the band pieces together their albums. Since Twenty One Pilots has been known to make concept albums with distinct storylines, I am interested to know if they tend to use a similar pattern of song styles/vibes between their albums in order to emulate the arc of a storyline. 


Visualizations
===================================================

Column {data-width=1000 .tabset}
----------------------------------------------------------------------

### Energy

```{r}

```
![](https://user-images.githubusercontent.com/60647028/74754427-df56a100-5271-11ea-9125-8f06fbd304ab.png)


### Tempo
![](https://user-images.githubusercontent.com/60647028/74755037-d1ede680-5272-11ea-86e0-d22d93645e57.png)

```{r}

```

Discussion
===================================================

Column {data-width=1000 .tabset}
-----------------------------------------------------------------------

Though there is certainly deviation, it appears as though there may exist a pattern of change between tracks for both energy and tempo that is present in each of the different albums. Based on the general pattern of peaks and divots in the graphs the pattern is as follows.

| Between Track #'s... | Energy | Tempo |
| :------------------- | :----: | :---: |
| 1 and 2 | increase | decrease |
| 2 and 3 | decrease | decrease |
| 3 and 4 | increase | increase |
| 4 and 5 | decrease | no clear pattern |
| 5 and 6 | no clear pattern | increase |
| 6 and 7 | no clear pattern | no clear pattern |
| 7 and 8 | decrease | decrease |
| 8 and 9 | increase | increase |
| 9 and 10 | increase | no clear pattern |
| 10 and 11 | decrease | no clear pattern |
| 11 and 12 | decrease | decrease |
| 12 and 13 | decrease | decrease |
| 13 and 14 | decrease | increase |

In regards to any deviation or unclear pattern - I would like to note that one of the albums, Vessel, has fewer songs than the others and therefore may exhibit the same general arc but have missing sections in the middle. I plan to review this possibility in further analyses. 

```{r}

```


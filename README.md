# igndata
Analysis on IGN ranking of videogames


## 20 years of games
Our initial goal is to determine if there are some temporal trends in the videogame industry ruled by the genre of the games.
For doing so, we took a dataset of [IGN](http://www.ign.com/games/reviews) reviews on videos games published since 20 years.

The dataset can be found on the [kaggle](https://www.kaggle.com/egrinstein/20-years-of-games) website.


The first question we can ask is if there is a global trend along the years. Games are reviewed by IGN journalists and graded from 0 to 10. 
We decided to plot the mean of notes, grouped by year, along with a boxplot to identify the first and third quartiles.

![Mean of Notes](plots/year_note.png)

The first analysis we make from this plot is that the notes are in average pretty high. It is always above 5 over 10. We notice that no year is especially better or worst than the others, even if notes of some years are sometimes more concentrated around the mean. 

We decided to go further in the analysis of the global trend of 20 years.
The next graph presents the number of games published, with the appreciation they received. The appreciation is directly linked with the note.

 - 10 is a Masterpiece
 - 9-9.9 is Amazing
 - 8-8.9 is Great
 - 7-7.9 is Good
 - 6-6.9 is OK
 - 5-5.9 is Mediocre
 - 4-4.9 is Bad
 - 3-3.9 is Awful
 - 2-2.9 is Painful
 - 1-1.9 is Unbearable
 - 0-0.9 is Disaster
![Number of games per year, with appreciation](plots/number per year - stacked.png)

The informations added by this plot is the fact that the number of games per year is extremely varying. As expected, there was very few games in 1995, because it was the beginning of the industry. We can notice a huge production in 2008. Rather suprisingly, it is decreasing after 2008. It can be explained by the dataset provenance. Indeed, it is reviews from a website, and it has been made before the end of 2016. So we can conclude that many games from the last 3-4 years haven't been reviewed yet.

![Appreciation of games along the years](plots/number per year - divided.png)

In this plot, we can confirm that the majority of games are reviewed as good, and great.


##Variations with months
We are now interested of the tendance during the year. Are the games published uniformely during the year, or is there pics ?

![Number of Release along the year](plots/game_month.png)
![Appreciations along the year](plots/number per month - stacked.png)

As we can see in these plot, we notice a huge number of release in november, and two small pics in March and in June. The pic of November can be explained by the proximity with Christmas.

![Mean of Notes along the year (Zoom)](plots/mean_month.png)

It is interesting to notice that even if the majority of games are released before Christmas, the best marked games are published in September. However we cannot really conclude because the difference in mean, and the first and third quartile is not extremely visible as we can see in the next plot.
![Mean of Notes along the year](plots/score per month.png)

##Editors and platform

Another way to study this dataset is to focus on the platforms and the editors.
![Evolution of platforms during 20 years](plots/score per year.png)

With the years, platforms have evolved, and some might not be available anymore. 
This is seen if we study the variations of colors from left to right. However, if we see the graph from top to bottom, we cannot conclude that a platform have noticeably received better critics than another.

We decided to focus our study on two majors producers, Nitendo and Sony.

![Platforms of Nitendo](plots/Nintendo/nintendo per year.png)

As said previously, we can noticed the living time of each console, and the overlapping between two generations of consoles.
The Wii is the console where most games have been produced, but also the worst.
It is to notice that games that are published nowadays are often published on several generations of consoles, the Wii, the Wii U and now the Switch, but the dataset doesn't seems to have registered all the supported platforms.


Let's now look at the second major publisher, Sony.
![Platforms of Sony](plots/Sony - PlayStation/Sony per year.png)

There is not remarquable variations among the platforms.

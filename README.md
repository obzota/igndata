# igndata
Analysis on IGN ranking of videogames


# First approach

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


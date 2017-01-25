# igndata
Analysis on IGN ranking of videogames


# First approach

Our initial goal is to determine if there are some temporal trends in the videogame industry ruled by the genre of the games.
For doing so, we took a dataset of [IGN](http://www.ign.com/games/reviews) reviews on videos games published since 20 years.

The dataset can be found on the [kaggle](https://www.kaggle.com/egrinstein/20-years-of-games) website.


The first question we can ask is if there is a global trend along the years. We decided to plot the mean of notes, grouped by year, along with a boxplot to identify the first and third quartiles.
![Mean of Notes](plots/year_note.png)

The first analysis we make from this plot is that the notes are in average pretty high. It is always above 5 over 10. We notice that no year is especially better or worst than the others, even if notes of some years are sometimes more concentrated around the mean. 



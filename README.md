## Project description
The aim of this project was to discover a correlation between a game's reception and its sale. We anticipated that a mutual relationship exists between such two aspects of a game, and a game with high sale is likely to be rated high. 

Before we chose this topic of research, we had several different options that we found interesting to research for it, but most of them were unable to collect enough data, or we couldn't find the correlation or causation. We all came to an agreement that we think this topic is interesting and reasonable. We were able to find the data that we needed and we could also go ahead and find correlation that might show the causation.

## Data description
Found in a well-known data community website "Kaggle," three data have been combined to produce the outcome of the project:
  
- [Data1](https://www.kaggle.com/destring/metacritic-reviewed-games-since-2000): Shows the ratings of the games that is shown by meta score and user score.
- [Data2](https://www.kaggle.com/rush4ratio/video-game-sales-with-ratings): Contains both ratings and sales. It has global sales data and also shows rating by the critic score and the user score.
- [Data3](https://www.kaggle.com/rgwegwegwe/vgsaledata): Gives both ratings and sales. It's rating is shown by the user score.
  
Then, ALL THREE DATA are merged into one that contains key informations of total sales and and user score. It also has informtions of the console, release date and name to help people see what is actually going on. 
   
See http://www.vgchartz.com/game/83196/grand-theft-auto-v/ to compare numbers to determine the units.

## Technology
Python 3 is the programming language that is selected mainly for inherent "pandas" and "matplotlib" libraries, which are useful to combine, operate, and visualize data. All contents of the project have been recorded and updated via an online web application Jupyter Notebook.

Documentations of the libraries can be found in:
- [pandas 0.24.2 documentation](https://pandas.pydata.org/pandas-docs/stable/getting_started/tutorials.html)
- [matplotlib 3.1.1 documentation](https://matplotlib.org/3.1.1/tutorials/introductory/usage.html)

## Analysis
![scatter plot 2](https://github.com/shpark61/data_science_project/blob/master/graphs/scatter%20plot%202.png)

Correlations of global sales by the user scores and critic scores are 0.09 and 0.24, respectively, which are not high enough to conclude that the sales are correlated to the scores. We thought some reviews could not be well-represented if there are too few reviews. This led us to filtering out to the average reviews where the number of reviews > 25.

![scatter plot 3](https://github.com/shpark61/data_science_project/blob/master/graphs/scatter%20plot%203.png)

The scatter plot above only employed data 2 which includes the number of users and critics, and dropped the data with number of users less than 25 and number of critics less than 20. Despite the removal, the graph shows similar trend to the data before confinement, presenting that the sales are influenced by the ratings given by both users and critics.

![line graph 1](https://github.com/shpark61/data_science_project/blob/master/graphs/line%20graph%201.png)

The line graph above employed a merged dataset from data 1,2,and 3 which includes the average number of global sales, user and critic score for each year from 1985 to 2016. The annual global sale was lucidly influenced by the advent of new games including Doom, Starfox, Street Fighter II, and Virtua Fighter which resulted into a huge spike around 1982 and reached its peak during the release of the renowned game, Pokemon.

![scatter plot 4](https://github.com/shpark61/data_science_project/blob/master/graphs/scatter%20plot%204.png)

The scatter plot above was created by a modified version of data 2 which contained only the sales of each regions (NA, EU, JP, Other), critic score, and user score. These scatter plots show a similarity with the other scatter plots mentioned above and do not show very close correlation between the scores and the actual regional sales. The highest correlation was found between NA sales and critic scores which perhaps hint toward more NA game players checking critic scores prior to purchasing games.

![scatter plot 1](https://github.com/shpark61/data_science_project/blob/master/graphs/scatter%20plot%201.png)

The scatter plot above employed the merged dataset of data 1,2,and 3 which was divided into smaller divisions of consoles. The global sales compared with user and critic score divided into consoles did not show great correlation. Sony, among the other types of gaming consoles, showed the greatest correlation between the global sales and scores.

## Conclusion

Through this project, we have discovered that consumers do not consider ratings of other users or critics when purchasing video games. Therefore, the hypothesis that a game with high sale is likely to be rated high is revealed to be false, as no clear correlation exist. A possible reasoning behind this result is the fact that customers are likley to leave ratings and reviews usually when they are dissatisfied with the game. Customers with strong feelings of the success or failure of the game will be more likely to leave reviews than those who are lukewarm regarding the game they played. 

## Possible Extensions

The extensions of this project could be to discover new factors—excluding ratings—that affect the sales of games. For instance, games with characters from movies or other media could attract the consumers better, earning more sales than the games which do not.


# NBA-Comparison-Algorithm

## How does it work?
This program will scrape the web for player data and tell you the three players that each player most embodies. The program works by selecting the most important features for each player, and creating a similarity metric using weighted euclidian distances. The population space consists of every player that has played at least 30 games since 1980.

## How do I use it?
Have a player in mind? Download the file and run the program to see their results. Make sure to replace the filepath with your own downloads of the csv data and replace the "players" variable with a list of the players you'd like to find comparisons on. Feed the players you're curious about as a list of strings to player_comp function and you should get the result within 2 seconds per player. All apostrophes and special foreign characters have been removed from player names. 

For example, running "player_comp(['Luka Doncic', 'Trae Young', Kobe Bryant'])" will return the following:

"Luka Doncic's comparison's are DeMar DeRozan, Tyreke Evans, and Carmelo Anthony.

Trae Young's comparison's are Isaiah Thomas, Stephon Marbury, and Damian Lillard.

Kobe Bryant's comparison's are Jerry Stackhouse, Dwyane Wade, and Vince Carter."

I found the results to be especially useful as a tool to better understand players from past eras who I never got to watch myself. For example, after scrolling through the results, I was able to draw comparisons and gained a greater appreciation for players like Jerry Stackhouse and Mitch Richmond.

## Only interested in results? 
Go straight to the complete list of results by opening the "Results" file. 





## Sources:
https://www.kaggle.com/justinas/nba-players-data?select=all_seasons.csv

https://www.kaggle.com/drgilermo/nba-players-stats

https://pypi.org/project/basketball-reference-web-scraper/

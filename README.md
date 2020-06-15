# NBA-Comparison-Algorithm

## How does it work?
This program will scrape the web for player data and tell you the three players that each player most embodies. The program works by selecting the most important features for each player, and creating a similarity metric using weighted euclidian distances. The population space consists of every player that has played at least 30 games since 1980.

## How do I use it?
Have a player in mind? Download the file and run the program to see their results. Make sure to replace the filepath with your own downloads of the csv data and replace the "players" variable with a list of the players you'd like to find comparisons on. Feed the players you're curious about as a list of strings to player_comp function and you should get the result within 2 seconds per player. All apostrophes and special foreign characters have been removed from player names. 
For example, running player_comp(['Luka Doncic', 'Trae Young', Kobe Bryant'] will return the following 

"Luka Doncic's comparison's are DeMar DeRozan, Tyreke Evans, and Carmelo Anthony
Trae Young's comparison's are Isaiah Thomas, Stephon Marbury, and Damian Lillard
Kobe Bryant's comparison's are Jerry Stackhouse, Dwyane Wade, and Vince Carter"

Only interested in results? Go straight to the results by opening the "Results" file. 





Sources:
https://pypi.org/project/basketball-reference-web-scraper/ to assist in scraping https://www.basketball-reference.com/ for player data
https://www.kaggle.com/justinas/nba-players-data?select=all_seasons.csv for biometric data on current players.
https://www.kaggle.com/drgilermo/nba-players-stats for biometric data on older players

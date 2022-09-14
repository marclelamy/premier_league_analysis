![alt text](https://github.com/marclelamy/premier_league_analysis/blob/main/docs:image/PL30-board-ball-and-Trophy-at-PL-launch.webp)


# Project Intro/Objective
This repo is about the Premier League analysis. I wanted to  understand more about the history of this League and so collected all the data about the games and players, cleaned it, conducted an analysis and wrote an [article on Medium](https://medium.com/@croissantboy/an-analysis-of-the-greatest-football-on-earth-interactive-article-74a057a82862) about it.


## Project Description
This project is decomposed into three sections (i.e three jupyter notebooks):
* Data collection: this was the process of collecting all the data about the games, the players and all the event that happened in every game likes goals, red/yellow cards, substitution, etc... I used the official website of the Premier League as main data source and after navigating through it, I understood how the data was display and the best way of getting it:
    * First, collect the ID of each season from a dropdown menu on the game pages
    * Loop through each season page (https://www.premierleague.com/.../{season_id}) to collect each game id
    * Loop through each game page (https://www.premierleague.com/.../{match_id}) to collect each game
    * Luckily for me, the website stored the games data (with players info, events, and a ton of other infos) in a JSON format readable in the html. I just had to flatten the json to have tabular data that I splitted in multiple files (games, events, players)

* Data cleaning: There was way too much information in those JSONs so I removed some columns, reformatted others and overall just cleaned the data to have a suitable format for the analysis (EDA).

* Data Analysis & Visualization: analyzed the data to find some interesting facts about the league. Not all insights have a viz but here are some viz that you can also find in html_viz and enjoy the interactibility as they're all made with Plotly!  


## Notes 
* To see the EDA.ipynb AND the different visualization, open [this html file](https://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/html_viz/eda.html)
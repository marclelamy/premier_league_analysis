![alt text](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/PL30-board-ball-and-Trophy-at-PL-launch.webp)


# Project Intro/Objective
This repo is about the Premier League analysis. I wanted to understand more about the history of this League and so collected all the data about the games and players, cleaned it, conducted an analysis, and wrote an [article on Medium](https://medium.com/@croissantboy/an-analysis-of-the-greatest-football-on-earth-interactive-article-74a057a82862) about it.


## Project Description
This project is decomposed into three sections (i.e three jupyter notebooks):
* Data collection: this was the process of collecting using webscraping, all the data about the games, the players, and all the events that happened in every game (goals, red/yellow cards, substitution, etc). I used the official website of the Premier League as the main data source and after navigating through it, I understood how the data was displayed and the best way of getting it:
    * First, collect the ID of each season from a dropdown menu on the games' pages
    * Loop through each season's page (https://www.premierleague.com/.../{season_id}) to collect each game id
    * Loop through each game's page (https://www.premierleague.com/.../{match_id}) to collect each game's data. Luckily for me, the website stores the game's data (with a lot more data that I needed) in a JSON format readable in the html. I just had to flatten the json to have tabular data that I splitted in multiple files (games, events, players)

* Data cleaning: There was way too much information in those JSONs so I removed some columns, reformatted others, dealed with missing values and generally cleaned the data to have a suitable format for the analysis (EDA).

* Data Analysis & Visualization: Definitely the most exciting and sexy to read! I analyzed the data to find some interesting facts about the league. Not all insights have a viz but here are some viz where you can enjoy the interactibility as they're all made with Plotly!  


## Notes 
* I couldn't managed to make the charts of the EDA notebook interactive on github so the only way to play with them is to run the EDA notebook or to check out some below.
* The EDA has a lot of insights that dont have charts, go take a look!


## Top 10 nicest charts and their link for interactibility with Plotly 
If you don't wanna run EDA.ipynb, check the charts below or in [docs/images](https://github.com/marclelamy/premier_league_analysis/tree/main/docs/images), you can open them by putting http://htmlpreview.github.io/? in front of http in the url.

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Distribution_of_events_over_the_minutes_of_the_games.html)
![Distribution_of_events_over_the_minutes_of_the_games](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Distribution_of_events_over_the_minutes_of_the_games.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Goals_vs_assists_per_season.html)
![Goals_vs_assists_per_season](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Goals_vs_assists_per_season.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Minutes_played_vs_goals_scores_vs_assists_vs_player's_position.html)
![Minutes_played_vs_goals_scores_vs_assists_vs_player's_position](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Minutes_played_vs_goals_scores_vs_assists_vs_player's_position.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Distribution_of_points_big_6_vs_other_teams.html)
![Distribution_of_points_big_6_vs_other_teams](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Distribution_of_points_big_6_vs_other_teams.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Number_of_time_each_team_has_finished_at_which_place_of_the_podium.html)
![Number_of_time_each_team_has_finished_at_which_place_of_the_podium](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Number_of_time_each_team_has_finished_at_which_place_of_the_podium.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Origin_of_the_players.html)
![Origin_of_the_players](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Origin_of_the_players.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Points_of_difference_with_the_team_ranked_after_itself.html)
![Points_of_difference_with_the_team_ranked_after_itself](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Points_of_difference_with_the_team_ranked_after_itself.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Ranking_of_the_Big_6_per_year.html)
![Ranking_of_the_Big_6_per_year](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Ranking_of_the_Big_6_per_year.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Ratio_Win_Draw_Lost_in_All_seasons_included.html)
![Ratio_Win,_Draw,_Lost_in_%_-_All_seasons_included](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Ratio_Win_Draw_Lost_in_All_seasons_included.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Cleansheets_per_season_(at_leat_10).html)
![Cleansheets_per_season_(at_leat_10)](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Cleansheets_per_season_(at_leat_10).png)
![alt text](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/PL30-board-ball-and-Trophy-at-PL-launch.webp)


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
* I could make the charts interactive on github so the only way to play with them is to run the EDA notebook.


## Top 10 nicest charts and their link for interactibility 
If you don't wanna run EDA.ipynb


[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Cleansheets_per_season_(at_leat_10).html)
![Cleansheets_per_season_(at_leat_10)](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Cleansheets_per_season_(at_leat_10).png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Distribution_of_events_over_the_minutes_of_the_games.html)
![Distribution_of_events_over_the_minutes_of_the_games](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Distribution_of_events_over_the_minutes_of_the_games.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Goals_vs_assists_per_season.html)
![Goals_vs_assists_per_season](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Goals_vs_assists_per_season.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Minutes_played_vs_goals_scores_vs_assists_vs_player's_position.html)
![Minutes_played_vs_goals_scores_vs_assists_vs_player's_position](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Minutes_played_vs_goals_scores_vs_assists_vs_player's_position.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Distribution_of_points_big_6_vs_other_teams_(in_%).html)
![Distribution_of_points_big_6_vs_other_teams_(in_%)](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Distribution_of_points_big_6_vs_other_teams_(in_%).png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Number_of_time_each_team_has_finished_at_which_place_of_the_podium.html)
![Number_of_time_each_team_has_finished_at_which_place_of_the_podium](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Number_of_time_each_team_has_finished_at_which_place_of_the_podium.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Origin_of_the_players.html)
![Origin_of_the_players](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Origin_of_the_players.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Points_of_difference_with_the_team_ranked_after_itself.html)
![Points_of_difference_with_the_team_ranked_after_itself](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Points_of_difference_with_the_team_ranked_after_itself.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Ranking_of_the_Big_6_per_year.html)
![Ranking_of_the_Big_6_per_year](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Ranking_of_the_Big_6_per_year.png)

[Link for interactibility](http://htmlpreview.github.io/?https://github.com/marclelamy/premier_league_analysis/blob/main/docs/html_viz/Ratio_Win,_Draw,_Lost_in_%_-_All_seasons_included.html)
![Ratio_Win,_Draw,_Lost_in_%_-_All_seasons_included](https://github.com/marclelamy/premier_league_analysis/blob/main/docs/images/Ratio_Win,_Draw,_Lost_in_%_-_All_seasons_included.png)



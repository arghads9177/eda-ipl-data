# Exploratory Data Analysis on IPL Datasets

## About Dataset
This dataset offers a rich resource for anyone interested in diving deep 
into the Indian Premier League (IPL), which is one of the premier 
franchise cricket leagues in India organized by the BCCI (Board of Control 
for Cricket in India). This tournament is held annually from March to May, 
featuring the best players from around the world competing for 8 different 
teams. Matches are played in various cities across India on a home and 
away basis.

The dataset contains information for 13 seasons, spanning from 2008 to 
2020. The IPL dataset comprises two main components:
- **Matches Dataset**
- **Ball-by-Ball Dataset**

These datasets collectively provide a comprehensive overview of IPL 
matches and detailed ball-by-ball action, enabling an in-depth analysis of 
various aspects of the game.

## Data Dictionary

### Matches Dataset
This dataset provides a high-level summary of each IPL match. The columns 
are as follows:
- **id (int64)**: Unique identifier for each match.
- **city (object)**: The city where the match was played.
- **date (object)**: The date on which the match was played.
- **player_of_match (object)**: The player awarded 'Player of the Match'.
- **venue (object)**: The stadium where the match was played.
- **neutral_venue (int64)**: Indicator if the venue was neutral (1) or not 
(0).
- **team1 (object)**: The first team competing in the match.
- **team2 (object)**: The second team competing in the match.
- **toss_winner (object)**: The team that won the toss.
- **toss_decision (object)**: The decision made by the toss winner (bat or 
field).
- **winner (object)**: The team that won the match.
- **result (object)**: The result of the match (e.g., normal, tie, no 
result).
- **result_margin (float64)**: The margin by which the match was won (runs 
or wickets).
- **eliminator (object)**: Indicates if the match was an eliminator or not 
(Y/N).
- **method (object)**: The method used if the match was decided by a 
method like Duckworth-Lewis.
- **umpire1 (object)**: Name of the first umpire.
- **umpire2 (object)**: Name of the second umpire.

### Ball-by-Ball Dataset
This dataset provides detailed information about every delivery bowled in 
each match. The columns are as follows:
- **id (int64)**: Match identifier to link with the matches dataset.
- **inning (int64)**: The inning number (1 or 2).
- **over (int64)**: The over number.
- **ball (int64)**: The ball number within the over.
- **batsman (object)**: The batsman's name.
- **non_striker (object)**: The non-striking batsman's name.
- **bowler (object)**: The bowler's name.
- **batsman_runs (int64)**: Runs scored by the batsman on that ball.
- **extra_runs (int64)**: Extra runs conceded on that ball.
- **total_runs (int64)**: Total runs scored on that ball (batsman runs + 
extra runs).
- **non_boundary (int64)**: Indicator if the runs were scored without a 
boundary (1) or with a boundary (0).
- **is_wicket (int64)**: Indicator if the ball resulted in a wicket (1) or 
not (0).
- **dismissal_kind (object)**: The method of dismissal (e.g., bowled, 
caught).
- **player_dismissed (object)**: The name of the dismissed player.
- **fielder (object)**: The fielder involved in the dismissal, if 
applicable.
- **extras_type (object)**: The type of extra runs (e.g., wide, no-ball).
- **batting_team (object)**: The batting team.
- **bowling_team (object)**: The bowling team.

## Problem Statement
### Understand Match Dynamics:
- Analyze the impact of factors like toss outcome, venue, and match 
context (eliminator, neutral venue) on match results.
- Investigate trends in win margins to identify the prevalence of close 
matches.

### Evaluate Player Performance:
- Identify standout performers through "Player of the Match" awards and 
explore their impact on winning teams.
- Analyze batting and bowling performances (strike rates, economy rates) 
from the ball-by-ball data to understand player strengths and weaknesses.


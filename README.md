- Project Overview

This project parses a chess tournament cross-table from a raw text file and produces a structured dataset.
The dataset contains the following fields for each player:

Name

State

Total Number of Points (Score)

Pre-Rating

Average Pre-Rating of Opponents

This fulfills the requirements from Project 1 (Data 607).

- Files in This Repository

tournamentinfo.txt – raw input file with tournament data.

Project1_Chess_Final.Rmd – R Markdown script to process the text file.

chess_players.csv – final output dataset with all players.

README.md – project description and instructions.

- How It Works

The .Rmd script reads the raw tournament file (from local copy or GitHub raw URL).

Each player’s information is stored in two rows in the text file:

Player row → name, total points, opponents.

State/rating row → state and pre/post rating.

Opponent IDs (from W, L, D markers) are mapped to pre-ratings.

The average opponent pre-rating is computed for each player.

Final dataset is saved to chess_players.csv and partially displayed in the knitted PDF/HTML (first 10 players).

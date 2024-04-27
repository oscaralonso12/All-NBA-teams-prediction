# All-NBA 2023-2024 Team Predictions

This repository contains code for predicting the All-NBA teams for the 2023-2024 NBA season based on statistical analysis.

## Dataset
The data used for this analysis was created by scraping box score, advanced stats, and historical All-NBA teams from Basketball Reference since the 1979 NBA season. The dataset includes various player statistics, including points, assists, rebounds, steals, blocks, player efficiency rating (PER), true shooting percentage (TS%), usage percentage (USG%), and win shares (WS). The analysis focuses on seasons starting from 1979 onwards, coinciding with the introduction of the NBA 3-point line.

## Data Preparation
- The full dataset is imported and split into training and test datasets.
- Training data excludes the 2023-2024 season.
- Test data includes only players who played at least 65 games in the 2023 season.

## Model Building
- The data is bootstrapped, and 1000 probit model are fitted to predict All-NBA selection.
- The distribution of estimates is visualized using histograms.
- Probabilities for each model are predicted and combined using the median across models.

## Results
Based on the calculated probabilities, the top 15 players are identified and classified into All-NBA teams.

## Table of All-NBA 2023 Team Predictions
![all-nba 2023-24 predictions]([https://github.com/oscaralonso12/All-NBA-teams-prediction/assets/41983149/a3b7f208-bce5-47c2-8e3e-594256677641](https://github.com/oscaralonso12/All-NBA-teams-prediction/blob/main/2024/all_nba_2024.qmd))](https://github.com/oscaralonso12/All-NBA-teams-prediction/assets/41983149/a3b7f208-bce5-47c2-8e3e-594256677641)

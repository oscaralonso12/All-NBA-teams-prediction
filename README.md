# All-NBA 2023-2024 Team Predictions

This repository contains code for predicting the All-NBA teams for the 2023-2024 NBA season based on statistical analysis.

## Dataset
The data used for this analysis was created by scraping box score, advanced stats, and historical All-NBA teams from Basketball Reference since the 1979 NBA season. The dataset includes various player statistics, including points, assists, rebounds, steals, blocks, player efficiency rating (PER), true shooting percentage (TS%), usage percentage (USG%), and win shares (WS). The analysis focuses on seasons starting from 1979 onwards, coinciding with the introduction of the NBA 3-point line.
![features_by_all_nba_historical](https://github.com/oscaralonso12/All-NBA-teams-prediction/assets/41983149/bb018a0b-2d6e-4fca-a189-b23533d54476)


## Data Preparation
- The full dataset is imported and split into training and test datasets.
- Training data excludes the 2023-2024 season.
- Test data includes only players who played at least 65 games in the 2023-2024 season.

## Model Building
- The data is bootstrapped, and 1000 probit model are fitted to predict All-NBA selection.
- The distribution of estimates is visualized using histograms.
- Probabilities for each model are predicted and combined using the median across models.

## Results
Based on the calculated probabilities, the top 15 players are identified and classified into All-NBA teams.

## Table of All-NBA 2023-2024 Team Predictions
[![all_nba_2023-2024_preds](https://github.com/oscaralonso12/All-NBA-teams-prediction/assets/41983149/6809d008-764f-48b8-88b1-5859b9c12268)](https://github.com/oscaralonso12/All-NBA-teams-prediction/blob/main/2024/all_nba_2024.qmd)

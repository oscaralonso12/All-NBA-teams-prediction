# All-NBA 2024-2025 Team Predictions

This repository contains code for predicting the All-NBA teams for the 2023–2024 NBA season using a Bayesian logistic regression model built with the `brms` package in R.

## Dataset
The data used for this analysis was created by scraping box score, advanced stats, and historical All-NBA teams from Basketball Reference since the 1979 NBA season. The dataset includes various player statistics, including points, assists, rebounds, steals, blocks, player efficiency rating (PER), true shooting percentage (TS%), usage percentage (USG%), and win shares (WS). The analysis focuses on seasons starting from 1979 onwards, coinciding with the introduction of the NBA 3-point line.
![features_by_all_nba_historical](https://github.com/oscaralonso12/All-NBA-teams-prediction/assets/41983149/e216e31a-ec5d-4d1e-a8f5-c3b58dd1ab1c)

## Data Preparation
- All numerical features are normalized using z-scores within each season, so that each stat reflects how a player compares to their peers in the same year.
- The full dataset is split into training and test datasets.
- Training data excludes the 2024-2025 season.
- Test data includes only players who played at least 65 games in the 2024-2025 season.

## Model Building
- A Bayesian logistic regression model is fit using the brms package, with predictors including season-normalized advanced stats such as VORP, Win Shares, and PER.
- The model is trained on historical data from 1979 through 2023.
- Posterior predictions are generated for players in the 2024–2025 season.
- For each player, the model estimates the probability of being selected to an All-NBA team.
- Posterior predictions are averaged across draws to produce final probability estimates for each player.

## Results
Based on the calculated probabilities, the top 15 players are identified and classified into All-NBA teams.

## Table of All-NBA 2024-2025 Team Predictions
![all_nba_2023-2024_preds](https://github.com/oscaralonso12/All-NBA-teams-prediction/assets/41983149/e3cf4fd1-5e2e-4bdf-ac3b-ebaff1c566b8)


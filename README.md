# Prediction-MPL-ID-S16-metode-Logistic-Regression
This project predicts the outcomes of Mobile Legends Professional League (MPL) matches using a Logistic Regression model.

## Overview
- The dataset consists of hardcoded match results from Week 1 and Week 2 of an MPL season.
- Team statistics such as match win rate, game win rate, and recent win/loss streaks are extracted and used as features.
- Features represent the difference in statistics between the two competing teams.
- A Logistic Regression model is trained on this data to classify which team is more likely to win a match.
- The trained model is then used to predict match outcomes for Week 3, simulating scores and updating team statistics accordingly.
- Finally, the project outputs the predicted standings after Week 3 based on the simulated results.

## Features Used
- Match Win Rate = Matches Won / Matches Played
- Game Win Rate = Games Won / (Games Won + Games Lost)
- Recent Streak = Sum of wins (+1) and losses (-1) in the last 3 matches

## How It Works

1. Initialize statistics for all teams based on Week 1 & 2 results.
2. Encode each match as a feature vector (difference in team statistics).
3. Train Logistic Regression on encoded matches with labels indicating the winning team.
4. Predict outcomes for Week 3 matches using the trained model.
5. Simulate match scores (2-0 or 2-1) based on predictions.
6. Update team statistics and generate final standings after Week 3.

## Usage
- Run the script to see predictions and updated standings.
- Modify the match results or week 3 fixtures as needed for other seasons.

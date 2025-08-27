🏏 Cricket Match Outcome Prediction
📖 Project Overview

This project focuses on predicting the outcomes of limited-overs cricket matches (T20 & ODI formats) using machine learning techniques. By analyzing a combination of historical match data, player performance statistics, and venue conditions, the model predicts which team is more likely to win a given match.

The purpose of this project is to demonstrate how data-driven insights can be applied to sports analytics, allowing analysts, enthusiasts, and researchers to better understand the key factors influencing match results.

📂 Dataset

The project integrates multiple cricket-related datasets containing both match-level and player-level information:

t20i_Matches_Data.csv → Match-level details (teams, venue, result, date, etc.)

t20i_Batting_Card.csv → Batting performance per player per innings

All datasets were cleaned, standardized, and merged to form a unified structure suitable for training predictive models.

⚙️ Methodology
🔹 Data Cleaning & Preprocessing

Removed abandoned/no-result matches

Standardized date, team, and venue formats

Created a binary target variable (1 = Team1 win, 0 = Team2 win)

Handled missing values and inconsistent records

🔹 Feature Engineering

Team Form: Rolling win percentage from the last 5 matches

Venue Effect: Encoded venue influence (home, away, neutral)

Player Performance Aggregates: Batting strike rate, bowling economy, partnerships, etc.

🔹 Model Training

Trained and compared multiple machine learning algorithms:

Logistic Regression

Random Forest

Gradient Boosting (XGBoost / LightGBM)

Evaluation was performed using cross-validation to ensure robustness.
 Evaluation Metrics

Models were assessed on:

Accuracy

Precision, Recall, F1-Score

ROC-AUC

Analysis revealed that recent player form and venue conditions were the most significant factors in predicting match outcomes.

🚀 Future Enhancements

Incorporate real-time weather data for better accuracy

Extend analysis to IPL and other franchise leagues

Deploy the model as a Streamlit/Flask web app for live predictions

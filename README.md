# Football Player Statistics Analyzer

![Football](football_half.jpg)

## Overview

This project provides tools for analyzing football (soccer) player statistics from the English Premier League 2023-2024 season. It includes two main components:

1. **Football Player Statistics Analyzer**: An interactive web application built with Streamlit that allows users to explore player statistics through visualizations and tables.

2. **Fantasy Premier League Points Calculator**: A Jupyter notebook that calculates fantasy points for players based on their performance metrics.

## Features

### Football Player Statistics Analyzer (Web App)

- **Interactive Filtering**: Filter players by team, position, age range, and minimum minutes played
- **Visualizations**:
  - Top scorers and assist providers
  - Goals vs. Expected Goals (xG) comparison
  - Progressive actions (carries, passes, runs)
  - Team contribution to goals and assists
  - Player age distribution
  - Position breakdown by team
  - Correlation heatmap of key statistics
- **Performance Analysis**:
  - Identify overperformers and underperformers based on goals vs. xG
  - View detailed player statistics
- **Data Export**: Download filtered data as CSV

### Fantasy Premier League Points Calculator

- Calculate fantasy points based on various performance metrics:
  - Goals and assists
  - Expected goals (xG) and expected assists (xAG)
  - Minutes played
  - Age (penalty for older players)
  - Yellow and red cards
  - Progressive actions (carries, passes, runs)

## Data Sources

The project uses the following data files:

- `premier-player-23-24.csv`: Contains detailed statistics for Premier League players from the 2023-2024 season
- `newpldata.csv`: Contains calculated fantasy points and player costs

## Installation

1. Clone this repository
2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

## Usage

### Running the Web App

```
streamlit run app.py
```

This will launch the Football Player Statistics Analyzer web application in your default browser.

### Using the Fantasy Points Calculator

Open the `CIA3FantasyPL.ipynb` notebook in Jupyter Notebook or Jupyter Lab to explore the fantasy points calculation and analysis.

## Stat Definitions

- **Gls**: Goals scored
- **Ast**: Assists
- **G+A**: Goals plus assists
- **xG**: Expected goals
- **npxG**: Non-penalty expected goals
- **xAG**: Expected assisted goals
- **PrgC**: Progressive carries (carries moving the ball towards the opponent's goal)
- **PrgP**: Progressive passes (passes moving the ball towards the opponent's goal)
- **PrgR**: Progressive runs (runs moving the ball towards the opponent's goal)
- **Min**: Minutes played
- **90s**: Number of 90-minute games played (Min / 90)
- **CrdY**: Yellow cards
- **CrdR**: Red cards
- **Per 90 Stats** (e.g., Gls_90): Metric per 90 minutes played

## License

This project is for educational purposes only.
# Premier League Multi-Season Performance Analytics

## Project Overview

This project explores Premier League team performance across three consecutive seasons: 2021/22, 2022/23, and 2023/24.

As a football enthusiast and Manchester City supporter, I wanted to go beyond league standings and understand how different teams performed across multiple seasons.

Using historical Premier League match data, I analyzed key performance indicators such as total points, goals scored, goals conceded, goal difference, and defensive performance.

I used Microsoft Excel for data preparation and Tableau to develop an interactive dashboard that allows users to compare teams, explore seasonal trends, and identify patterns in overall performance.

The goal of this project was to combine my interest in football with practical data analytics skills, focusing on data preparation, performance measurement, visualization, and communicating insights.


## Dashboard Preview

![Premier League Performance Trends Dashboard](images/dashboard_preview.png)

## Interactive Dashboard

View the interactive dashboard on Tableau Public:

[Open Tableau Public Dashboard](https://public.tableau.com/app/profile/parth.nag7346/viz/AnalysisofPremeirLeagueacross3seasonsaa/PremierLeaguePerformanceTrends202122202324)

## Key Features

- Season-specific team points rankings
- Goal difference comparison
- Three-season points progression
- Attacking versus defensive performance
- Champion, best attack, best defense, and clean-sheet KPI cards
- Interactive season filtering

## Dataset Structure

This project uses historical Premier League match data from three consecutive seasons: 2021/22, 2022/23, and 2023/24.

The dataset contains:

* **1,140 matches:** 380 matches from each season.
* **2,280 team-match records:** Each match is represented from both teams' perspectives.
* **60 team-season records:** Performance summaries for 20 clubs across each of the three seasons.

### Data Organization

The processed Excel workbook contains six worksheets:

| Worksheet           | Description                                                      |
| ------------------- | ---------------------------------------------------------------- |
| Project_Info        | Overview of the project and dataset                              |
| Data_Quality        | Summary of data completeness and record counts                   |
| Match_Level_Cleaned | Historical match results and match-level statistics              |
| Team_Match_Level    | Team-specific match statistics, including cumulative performance |
| Team_Summary        | Aggregated team performance metrics for each season              |
| Column_Dictionary   | Field definitions and descriptions                               |

### Key Performance Indicators

The analysis includes:

* Total points, wins, draws, and losses
* Goals scored, goals conceded, and goal difference
* Home and away performance
* Points per match and win percentage
* Shots, shots on target, and shot accuracy
* Goal conversion rate
* Clean sheets and defensive performance
* Season-over-season team performance

### Data Validation

The dataset was reviewed for completeness and consistency.

Validation checks confirmed:

* 380 match records per season.
* 20 clubs per season.
* 38 matches played per team in each season.
* No duplicate match IDs.
* No missing values in the essential match identification, team, score, and result fields reviewed.
* Consistent calculations for points, match results, and goal difference across all 60 team-season records.

These checks support the reliability of the dataset for descriptive performance analysis.

## Seasons Analyzed

- 2021/22
- 2022/23
- 2023/24

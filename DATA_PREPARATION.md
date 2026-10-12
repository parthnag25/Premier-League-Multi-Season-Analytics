# Data Preparation and Transformation

## 1. Overview

This document explains the data structure and transformations used in the Premier League Multi-Season Performance Analytics project.

The project analyzes match-level data from three Premier League seasons: 2021/22, 2022/23, and 2023/24.

The processed datasets support historical performance analysis and interactive Tableau visualizations.

## 2. Source Data

The repository contains three season-specific CSV datasets:

* `EPL_2021_22_raw.csv`
* `EPL_2022_23_raw.csv`
* `EPL_2023_24_raw.csv`

Each dataset contains 380 Premier League matches, resulting in 1,140 match records across the three seasons.

## 3. Cleaned Match-Level Dataset

The processed workbook contains a worksheet named `Match_Level_Cleaned`.

This dataset combines the three seasons into a consistent match-level structure.

It includes standardized fields for:

* Match identification
* Season and match date
* Home and away teams
* Full-time and half-time results
* Goals scored and conceded
* Shots and shots on target
* Fouls, corners, and disciplinary statistics

Each match is assigned a unique Match ID.

The dataset contains 1,140 match records.

## 4. Team-Match-Level Transformation

The `Team_Match_Level` worksheet converts match-level information into a team-focused analytical structure.

Each match is represented by two records:

1. One record for the home team.
2. One record for the away team.

This produces 2,280 team-match records.

The dataset includes calculated performance indicators such as:

* Goals For
* Goals Against
* Goal Difference
* Match Points
* Win, Draw, and Loss Flags
* Clean Sheet Flag
* Shot Accuracy Rate
* Goal Conversion Rate
* Cumulative Points
* Cumulative Goals

This structure allows team performance to be analyzed consistently across home and away fixtures.

## 5. Team-Season Aggregation

The `Team_Summary` worksheet contains aggregated performance metrics for each club in each season.

The dataset contains 60 team-season records, representing 20 clubs across three seasons.

Key metrics include:

* Matches Played
* Total Points
* Wins, Draws, and Losses
* Goals For and Goals Against
* Goal Difference
* Home and Away Performance
* Clean Sheets
* Points Per Match
* Win Rate
* Shot Accuracy and Goal Conversion Metrics

These metrics support comparisons between teams and across seasons.

## 6. Key Calculations

The analysis uses several performance calculations.

**Match Points**

* Win = 3 points
* Draw = 1 point
* Loss = 0 points

**Goal Difference**

Goal Difference = Goals For − Goals Against

**Points Per Match**

Points Per Match = Total Points / Matches Played

**Win Rate**

Win Rate = Wins / Matches Played

**Shot Accuracy Rate**

Shot Accuracy Rate = Shots on Target / Total Shots

**Goal Conversion Rate**

Goal Conversion Rate = Goals Scored / Total Shots

Rates are stored as decimal values and can be displayed as percentages.

## 7. Data Quality

The processed workbook includes a `Data_Quality` worksheet summarizing data completeness and record counts.

Key checks include:

* 380 matches per season
* 20 clubs per season
* 38 matches per club per season
* Consistency between match results and points calculations
* Consistency between goals scored, goals conceded, and goal difference

The workbook also includes a `Column_Dictionary` worksheet documenting dataset fields.

## 8. Tableau Integration

The processed Excel workbook is structured for Tableau analysis.

The team-level datasets support:

* League performance comparisons
* Points progression across seasons
* Attacking and defensive comparisons
* Goal-difference analysis
* Interactive KPI dashboards

The finished interactive dashboard is available through Tableau Public.

## 9. Documentation Scope

This document describes the structure and calculations observable in the processed workbook.

The specific sequence of Excel operations used during the original cleaning process has not yet been independently reconstructed.

Further documentation may be added to explain the original source locations, preparation tools, and detailed cleaning decisions.

# Data Validation and Quality Checks

## 1. Overview

Data validation was performed to assess the internal consistency of the Premier League Multi-Season Performance Analytics dataset.

The analysis covers three Premier League seasons:

* 2021/22
* 2022/23
* 2023/24

The validation focuses on team-season performance metrics, including match results, points, goals, and home/away performance.

## 2. Dataset Summary

The processed dataset contains:

* 1,140 match-level records
* 2,280 team-match-level records
* 60 team-season summary records
* 20 clubs per season
* 38 matches per club per season

## 3. Team-Season Validation

Five consistency checks were performed on all 60 records in the `Team_Summary` worksheet.

| Validation Check                             | Records Checked | Discrepancies |
| -------------------------------------------- | --------------: | ------------: |
| Wins + Draws + Losses = Matches Played       |              60 |             0 |
| Points = (3 × Wins) + Draws                  |              60 |             0 |
| Goals For − Goals Against = Goal Difference  |              60 |             0 |
| Home Matches + Away Matches = Matches Played |              60 |             0 |
| Home Points + Away Points = Total Points     |              60 |             0 |

All five checks passed for every team-season record.

## 4. League-Wide Goal Reconciliation

For each season, the total number of goals scored across all teams should equal the total number of goals conceded.

| Season  | Total Goals Scored | Total Goals Conceded |
| ------- | -----------------: | -------------------: |
| 2021/22 |              1,071 |                1,071 |
| 2022/23 |              1,084 |                1,084 |
| 2023/24 |              1,246 |                1,246 |

All three seasons passed the league-wide goal reconciliation check.

## 5. Interpretation

These results demonstrate that the core team-season performance metrics are internally consistent.

The validation supports the use of the processed dataset for:

* Historical league performance comparisons
* Team points analysis
* Goal-difference comparisons
* Home and away performance analysis
* Multi-season Tableau visualizations

## 6. Validation Limitations

These checks focus on arithmetic consistency within the processed team-season dataset.

They do not constitute a complete audit of:

* Every match-level source record
* The original data collection process
* All optional statistical fields
* Every calculated Tableau measure
* Historical changes resulting from official points deductions

Additional validation would be required to establish the accuracy of those elements.

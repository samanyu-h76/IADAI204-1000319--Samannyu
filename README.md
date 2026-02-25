# IPL Match Analysis Dashboard — Data Storytelling with Tableau

## Project Overview

This project analyses IPL cricket data using Tableau to identify performance trends, rivalry dynamics, and match-winning factors. The objective was to transform raw sports data into an interactive dashboard that delivers actionable insights through visual storytelling.

The analysis explores:

- Top-performing batsmen and bowlers
- Team rivalries and dominance patterns
- Toss decision impact on match outcomes
- Venue-based performance trends

The final output is an interactive Tableau dashboard designed for coaches, analysts, broadcasters, and fans.

---

## Purpose and Target Audience

### Purpose

- Identify key player performance trends.
- Analyse head-to-head team rivalries.
- Understand how toss decisions and venues influence match outcomes.
- Present insights through interactive visual storytelling.

### Target Audience

- IPL teams and coaching staff
- Sports analysts and broadcasters
- Cricket fans interested in data-driven insights

---

## Data Summary

Two datasets were used:

- **matches.csv** — match-level information (teams, venues, toss decisions, winners).
- **deliveries.csv** — ball-by-ball performance data.

### Data Join

The datasets were joined in Tableau using:
matches.id = deliveries.match_id


An inner join ensured accurate integration of match-level and ball-level information.

---

## Data Cleaning and Preprocessing

The following preprocessing steps were performed:

- Standardised team names to remove inconsistencies.
- Created cleaned fields:
  - Clean Team1
  - Clean Team2
  - Clean Winner
  - Clean Venue
- Handled missing values using consistent labels.
- Removed unnecessary columns (e.g., umpire fields).
- Structured data to prevent duplication issues from ball-level joins.

### Key Calculated Fields

- Toss Winner Won Match (binary indicator)
- Team1 Win Flag
- Valid Wicket (excluding run-outs)
- Strike Rate (runs per 100 balls)
- Economy Rate (runs conceded per over)
- Dot Ball Percentage

Win percentages were calculated using distinct match counts to avoid inflated metrics.

---

## Exploratory Data Analysis (EDA)

### 1. Player Performance

- Top batsmen identified using total runs and strike rate.
- Top bowlers analysed using wickets and economy rate.
- Findings indicate that elite players consistently dominate performance metrics.

### 2. Team Rivalries

- Heatmap visualisation used to compare head-to-head matchups.
- Analysis reveals uneven rivalry dominance patterns between certain teams.

### 3. Toss Decision Impact

- Line charts show how toss decisions influence win probability across seasons.
- Field-first strategies demonstrate relatively stable performance.

### 4. Venue Impact

- Match distribution varies across venues.
- Teams such as Mumbai Indians (MI) and Rajasthan Royals (RR) show strong winning presence at specific stadiums, suggesting familiarity advantages.

---

## Dashboard Features

- Interactive filters for season, team, venue, and toss decision.
- Bar charts for player performance analysis.
- Heatmaps for rivalry comparison.
- Line charts for toss decision trends.
- Venue performance visualisations.
- Structured layout using containers for improved storytelling.

---

## Key Insights

- Elite batsmen contribute disproportionately to total runs.
- Leading bowlers maintain consistent wicket-taking impact.
- Rivalry analysis reveals dominant head-to-head matchups.
- Toss decisions influence outcomes but do not guarantee success.
- Venue familiarity appears to contribute to team performance, especially for MI and RR.

---

## Conclusion

This project demonstrates how sports analytics can transform raw data into meaningful insights through data preparation, analysis, and visual storytelling. The interactive dashboard enables stakeholders to explore IPL match dynamics from multiple perspectives.

### Future Improvements

- Integration of advanced player metrics.
- Inclusion of pitch condition or weather data.
- Predictive modelling for match outcomes.

---
## Link for the published Tableau Public
https://public.tableau.com/views/IPLPerformanceAIunit-4SA/Storyboard?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

---
## Repository Contents

- Data folder (Datasets)
- Tableau dashboard file (.twbx)
- README documentation

---

## Author Information

Name: Samanyu H
Course: Artificial Intelligence  
Project: The Art of Storytelling with Data  

# 🏏 IPL Analysis Dashboard (2008–2022)

## Overview
This repository features an interactive **Power BI dashboard** analysing IPL player and match performance from **2008 to 2022**, covering 950 matches and 225,000+ deliveries. The base dashboard was built following a guided tutorial to learn Power BI fundamentals; the **Toss & Scoring Insights** page was designed and built independently, using custom DAX measures to answer questions the base dashboard doesn't cover.

---

## 📊 Key Highlights

### 🏆 Season KPIs
- IPL Winner
- Orange Cap (Most Runs in a Season)
- Purple Cap (Most Wickets in a Season)
- Total Sixes & Fours Hit

---

## 🧢 Player Performance

### Batting Stats
- Total Runs
- Number of Sixes & Fours
- Strike Rate (runs scored per 100 balls)

### Bowling Stats
- Wickets Taken
- Economy Rate (runs conceded per over)
- Bowling Average (runs conceded per wicket)
- Bowling Strike Rate (balls bowled per wicket)

---

## 📈 Match & Team Insights
- Matches Won by Venue (Runs vs Wickets)
- Total Wins by Team (Season-wise)
- Matches Won Based on Toss Decision
- Matches Won by Runs vs Wickets

---

## 🔍 Extended Analysis: Toss Impact, Scoring Trends & Team Consistency

Building on the base dashboard, I added an independent analysis page using custom DAX measures, covering all 950 matches and 225,000+ deliveries from 2008 to 2022.

![Toss and Scoring Insights](toss_scoring_insights.png)

### Key Findings

- **Toss decision matters more than winning the toss.** Overall, toss winners only went on to win 51.7% of matches — close to a coin flip. However, the decision made after winning the toss had a real effect: teams that elected to **field first won 55.4%** of matches, compared to **45.4% when electing to bat first**.
- **Scoring has risen over time.** Average innings totals climbed from 154.6 runs (2007/08) to 164.8 runs (2022) — a 6.6% increase — with 2018 and 2022 standing out as the highest-scoring seasons.
- **Chennai Super Kings are the most consistently strong team.** Across 13 seasons, CSK combine a high win rate (59%) with low season-to-season variability, visualised in the heatmap above. Newer franchises such as Lucknow Super Giants show strong early win rates, but these are based on only 1–2 seasons and aren't directly comparable to franchises with a longer track record.

### DAX Measures Used

- `Toss Win %` — win rate split by toss decision (bat vs. field)
- `Avg Innings Score` — average runs per innings, aggregated by season
- `Team Win %` — team-level win rate by season, used to build the consistency heatmap

---

## 🎯 Purpose
This dashboard demonstrates the ability to:
- Analyse player and team performance across 15 seasons of match data
- Compare batting and bowling efficiency using derived metrics
- Independently design and test hypotheses (toss decision, scoring trends, team consistency) using DAX
- Communicate findings clearly through visual design, including conditional-formatting heatmaps

---

## 🛠 Tools Used
- Power BI (Data Modelling, DAX, Interactive Visualisations)
- SQL (PostgreSQL — table creation and CSV import)
- Power Query (data shaping and unpivoting for team-level analysis)

---

## 📎 Notes
This project demonstrates how sports data can be transformed into meaningful insights using Power BI — from guided fundamentals through to independently designed statistical analysis.

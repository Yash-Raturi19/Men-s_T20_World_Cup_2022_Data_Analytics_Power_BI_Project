# Men-s_T20_World_Cup_2022_Data_Analytics_Power_BI_Project

# 🏏 ICC Men's T20 World Cup 2022 Data Analytics | Power BI Project

## Table of Contents

* Problem Statement
* Data Source
* Data Collection
* Data Transformation
* Data Modeling
* DAX Measures
* Dashboard Reports
* Tools & Technologies
* Project Insights
* References

---

# Problem Statement

This project aims to analyze the ICC Men's T20 World Cup 2022 and identify the best-performing players using data-driven insights. The dashboard enables users to evaluate batting, bowling, and all-round performances and select the strongest Playing XI based on predefined performance criteria.

---

# Data Source

Data was collected from multiple cricket statistics sources:

* ESPN Cricinfo
* ICC T20 World Cup Records
* Bright Data

The dataset contains:

* Match Summary
* Batting Statistics
* Bowling Statistics
* Player Information
* Team Performance Data

---

# Data Collection

Data was extracted using web scraping techniques.

### Process:

1. Scraped match and player statistics.
2. Converted JSON data into structured datasets.
3. Processed data using Python and Pandas.
4. Exported cleaned datasets into CSV format.

---

# Data Transformation

Data cleaning and preprocessing included:

* Handling missing values
* Removing duplicates
* Standardizing player names
* Data type corrections
* Match ID mapping
* Feature engineering
* Power Query transformations

---

# Data Modeling

Created relationships between multiple tables:

* Match Summary
* Batting Summary
* Bowling Summary
* Player Information

Implemented a Star Schema model to improve dashboard performance and analytical capabilities.

---

# DAX Measures

### Batting Metrics

```DAX
Total Runs =
SUM(Batting_Summary[Runs])

Batting Average =
DIVIDE([Total Runs],[Dismissals],0)

Strike Rate =
DIVIDE([Total Runs],[Balls Faced],0)*100

Boundary Percentage =
DIVIDE([Boundary Runs],[Total Runs],0)*100
```

### Bowling Metrics

```DAX
Total Wickets =
SUM(Bowling_Summary[Wickets])

Economy Rate =
DIVIDE([Runs Conceded],([Balls Bowled]/6),0)

Bowling Average =
DIVIDE([Runs Conceded],[Total Wickets],0)

Bowling Strike Rate =
DIVIDE([Balls Bowled],[Total Wickets],0)
```

### Additional Metrics

```DAX
Dot Ball Percentage =
DIVIDE([Dot Balls],[Balls Bowled],0)*100

Matches Played =
DISTINCTCOUNT(Match_Summary[Match_ID])
```

---

# Dashboard Reports

## 🏏 Team Analysis

* Total Matches
* Win Percentage
* Team Comparison
* Tournament Performance

## 🥇 Openers Analysis

Selection Criteria:

* Batting Average > 30
* Strike Rate > 140
* Boundary % > 50

## 🎯 Middle Order Analysis

Selection Criteria:

* Average > 40
* Strike Rate > 125
* Average Balls Faced > 20

## ⚡ Finisher Analysis

Selection Criteria:

* Strike Rate > 130
* Average > 25
* Match Finishing Ability

## 🔄 All-Rounder Analysis

Selection Criteria:

* Batting Contribution
* Bowling Contribution
* Economy < 7

## 🎳 Specialist Fast Bowlers

Selection Criteria:

* Economy < 7
* Bowling Average < 20
* Dot Ball % > 40

## 🏆 Best Playing XI

Final selection of the best-performing players based on statistical analysis.

---

# Project Insights

### Key Findings

* Identified the most impactful batters and bowlers.
* Compared player performances using advanced cricket metrics.
* Built an optimal Playing XI using data-driven criteria.
* Created interactive visualizations for performance comparison.

---

# Dashboard Preview

## Team Performance Dashboard

(Add Screenshot Here)

## Player Analysis Dashboard

(Add Screenshot Here)

## Best Playing XI Dashboard

(Add Screenshot Here)

---

# Tools & Technologies

* Power BI
* Power Query
* DAX
* Python
* Pandas
* Jupyter Notebook
* Beautiful Soup
* Excel

---

# Project Structure

```text
📂 T20-WorldCup-2022-Analytics
│
├── Dataset
├── Power BI Dashboard (.pbix)
├── Screenshots
├── Python Notebook
├── CSV Files
└── README.md
```

---

# References

* ESPN Cricinfo
* ICC Men's T20 World Cup 2022
* Bright Data
* Power BI Documentation

---

## Author

**Yash R**

📊 Data Analyst | Power BI Developer

* LinkedIn: Add Your Profile Link
* GitHub: Add Your GitHub Link

⭐ If you found this project useful, don't forget to star the repository!

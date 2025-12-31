# Impact of Exam Period on Daily Habits  
### A Time-Series Exploratory Data Analysis

## Project Overview
During semester examination periods, students often significantly alter their daily routines — increasing study hours while compromising sleep, leisure, and physical activity. This project analyzes one month of self-tracked daily habit data (November 2025, a semester exam month) to understand how exam-driven study intensity impacts sleep, screen time, exercise, and overall lifestyle balance.

The goal of this project is to apply structured data analytics techniques to a real-world dataset and extract meaningful behavioral insights through exploratory data analysis (EDA) and visual storytelling.

---

## Problem Statement
How does an exam-heavy academic period affect daily habits such as sleep, screen time, study duration, and exercise?

Specifically:
- Do increased study hours correlate with reduced sleep or higher screen time?
- How do habits vary across exam and non-exam days?
- Are there observable weekly trends during the exam month?
- Which days appear most balanced versus most strained?

---

## Dataset Description

- **Source:** Self-tracked data recorded using Google Sheets  
- **Time Period:** November 2025 (30 days)  
- **Granularity:** Daily  
- **Context:** November was a semester examination month. Student uses phone/laptop to studying and course, so the screen time includes them both.

### Tracked Variables
- Sleep duration (hours)
- Screen time (hours)
- Course study hours
- Curriculum study hours

### Semester Exam Dates
The following dates were semester examination days:
- **November 14**
- **November 15**
- **November 17**
- **November 19**
- **November 29**

These dates provide important contextual markers for interpreting behavioral changes.

---

## Tools & Technologies Used
- **Google Sheets** – Data collection
- **Python**
  - NumPy – Data manipulation and statistical analysis
  - Matplotlib – Data visualization
- **Calendar module** – Calendar-accurate weekly grouping

---

## Data Cleaning & Preparation
Since, I recorded the data on my own, there weren't many irrelevant entries but still I followed the necessary data cleaning and pre-processing steps.
The following steps were performed before analysis:
- Exported data from Google Sheets as CSV
- Extracted calendar day values for time-series and weekly analysis
- Grouped data using calendar-based weeks instead of fixed intervals

---

## Exploratory Data Analysis (EDA)

The analysis focuses on:
- Descriptive statistics for each habit (mean, median, variance)
- Day-to-day trends across the month
- Correlation analysis between sleep, screen time and study hours
- Comparison between high-sleep and low-sleep days
- Identification of best and worst study days
- Calendar-based weekly habit trends

---

## Visualizations
The following visualizations were created to support insights:
- Sleep duration trend over time
- Study hours trend (course vs curriculum)
- Screen time trend
- Study efficiency over time
- Stacked bar chart of total study hours
- Weekly averages based on calendar weeks

Each visualization is designed to answer a specific analytical question and support data-driven storytelling.

---

## Key Insights (Summary)
Some high-level insights observed from the analysis include:
- Study hours increased significantly during exam weeks, with higher variability in sleep duration.
- High-sleep days were generally associated with lower screen time and improved study efficiency.
- Screen time tended to spike on days with lower course study, suggesting possible fatigue or burnout.
- Balance scores declined toward peak exam periods, indicating cumulative strain.
- Weekly trends show the most intensive study load occurred mid-month, aligning with exam dates.

(*Detailed insights are supported by visualizations in the analysis script.*)

---

## Limitations
- Data represents a single individual and may not generalize broadly.
- November is an exam-heavy month, which introduces seasonal bias.
- Data is self-reported and subject to human error.
- Academic performance outcomes (e.g., grades) were not included.

---

## Future Improvements
- Compare exam months with non-exam months
- Add mood, energy, or focus scores for deeper behavioral analysis
- Automate data collection
- Expand dataset to multiple participants
- Build an interactive dashboard using Tableau, Power BI, or Streamlit

---

## Repository Contents
- `/data` – Raw dataset (CSV)
- `/analysis` – Python analysis script
- `/visuals` – Generated charts and figures (to be added)

---

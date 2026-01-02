# Impact of Exam Period on Daily Habits  
## A Time-Series Exploratory Data Analysis

## 📌 Project Overview
During semester examination periods, students often restructure their daily routines — increasing exam-focused study while attempting to balance sleep, leisure, and long-term learning goals. This project analyzes one month of self-tracked daily habit data (November 2025, a semester exam month) to understand how exam pressure influences productivity, recovery, and leisure behavior.

The project applies structured data analytics techniques to a real-world dataset, emphasizing exploratory data analysis (EDA), feature engineering, and calendar-aware trend analysis.

---

## 🎯 Problem Statement
How does an exam-heavy academic period affect the balance between:
- **Exam preparation (curriculum study)**,
- **Long-term skill development (online course study)**,
- **Sleep (recovery)**, and
- **Leisure (non-productive screen time)**?

Specifically:
- How do study patterns differ between exam days and non-exam days?
- Does exam preparation crowd out sleep, leisure, or long-term learning?
- Are there observable weekly trends in behavior during the exam month?
- Which days appear most balanced versus most strained?

---

## 📊 Dataset Description

- **Source:** Self-tracked data recorded using Google Sheets  
- **Time Period:** November 2025 (30 days)  
- **Granularity:** Daily  
- **Context:** Semester examination month  

### Tracked Variables

| Variable | Description |
|--------|------------|
| Sleep (hours) | Total daily sleep duration |
| Course Study (hours) | Time spent learning an online course (long-term skill development) |
| Curriculum Study (hours) | Time spent studying for semester exams |
| Leisure (hours) | Non-productive screen time (entertainment, passive browsing, etc.) |

### Semester Exam Dates
The following dates were official semester examination days:
- **November 14**
- **November 15**
- **November 17**
- **November 19**
- **November 29**

These dates are used as contextual markers for comparative analysis.

---

## 🧰 Tools & Technologies Used
- **Google Sheets** – Data collection
- **Python**
  - NumPy – Data manipulation, statistics, and feature engineering
  - Matplotlib – Data visualization
- **Calendar module** – Calendar-accurate weekly grouping
- **Google Colab** - For running the analysis scripts
---

## 🧹 Data Cleaning & Processing
Several data processing steps were performed to improve analytical validity:
- Exported raw data from Google Sheets to CSV format
- Identified and corrected a mixed “screen time” variable by separating productive study time from non-productive leisure time
- Removed unreliable exercise data due to inconsistent logging
- Handled missing values by converting empty entries to NaN
- Converted numeric columns to floating-point values
- Extracted calendar day values for time-series and weekly analysis
- Grouped data using calendar-based weeks rather than fixed intervals

These steps ensured that the analysis accurately reflects meaningful behavioral patterns.

---

## 🔍 Exploratory Data Analysis (EDA)

The analysis focuses on:
- Descriptive statistics for each habit
- Daily time-series trends across the month
- Comparison of exam days versus non-exam days
- Correlation analysis between sleep, study types, and leisure
- Identification of best and worst productivity days
- Calendar-based weekly habit trends
- Study efficiency analysis
- Balance score analysis capturing trade-offs between productivity, recovery, and leisure

---

## 📈 Visualizations
The following visualizations were created to support analytical insights:
- Sleep duration trend over time
- Curriculum study (exam prep) vs course study trends
- Leisure time trend
- Study efficiency over time
- Balance score
- Stacked bar chart of total productive study hours

Each visualization is designed to answer a specific analytical question and support data-driven storytelling.

---

## 💡 Key Insights (Summary)
High-level insights observed from the analysis include:
- Exam preparation hours increased significantly around exam dates, while online course study time showed greater variability.
- Leisure time generally decreased during peak exam periods, suggesting intentional behavioral trade-offs.
- High curriculum-study days were often associated with reduced sleep and lower leisure time.
- Weeks with clustered exams showed the highest study intensity and the lowest balance scores.
- Long-term learning (online course study) was deprioritized during peak exam stress, highlighting opportunity costs during short-term academic pressure.

(*Detailed insights are supported by visualizations and statistical outputs in the analysis scripts.*)

---

## ⚠️ Limitations
- Dataset represents a single individual and may not generalize broadly.
- November is an exam-heavy month, introducing seasonal bias.
- Data is self-reported and subject to measurement error.
- Academic performance outcomes (e.g., exam scores) were not included.
- Amateur data analysis (I am still learning, and I just wanted to test my analysis skills)

---

## 🚀 Future Improvements
- Compare exam months with non-exam months
- Introduce mood, energy, or focus ratings
- Automate data collection
- Expand dataset to multiple participants
- Build an interactive dashboard using Tableau, Power BI, or Streamlit

---

## 📁 Repository Contents
- `/data` – Raw dataset (CSV)
- `/analysis` – Python analysis scripts
- `/visuals` – Generated charts and figures

---

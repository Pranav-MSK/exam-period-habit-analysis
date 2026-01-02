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
- **Context:** Semester examination month habit (hrs) recorded
- *Note: I use my phone and laptop for studying, so the curriculum and course study hours are also the time spent with a screen*

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
- Sleep duration trend over time ![📈](visuals/Sleep%20Trend.png)
- Curriculum study (exam prep) vs course study trends ![📈](visuals/Study%20Trends.png)
- Leisure time trend ![📈](visuals/Leisure%20Time%20Trend.png)
- Study efficiency over time ![📈](visuals/Focus%20Ratio%20Over%20Time.png)
- Balance score ![📈](visuals/Balance%20Score.png)
- Stacked bar chart of total productive study hours ![📊](visuals/Productive%20Hours.png)

Each visualization is designed to answer a specific analytical question and support data-driven storytelling.

---

## 💡 Final Insights

This analysis explored how daily habits shifted during a semester examination month by examining sleep, exam preparation, online course study, and leisure behavior. Several clear patterns emerged:

**1. Exam Period Significantly Reshaped Time Allocation**  
During November, time was reallocated primarily toward **curriculum study (exam preparation)**. Curriculum study hours increased noticeably on and around official exam dates. Long-term online course study became more inconsistent and was often deprioritized during peak exam periods. Leisure time generally declined near exam days, indicating intentional trade-offs under academic pressure.

**2. Exam Days vs Non-Exam Days Show Distinct Behavior**  
Comparing exam days with non-exam days revealed clear contrasts:
- Curriculum study hours were substantially higher on exam days.
- Leisure time was consistently lower on exam days.
- Sleep showed a mild decline around exams, indicating partial sacrifice of recovery.

These differences highlight how academic pressure changes daily routines.

**3. Trade-Offs Between Productivity and Leisure**  
Correlation analysis revealed:
- Higher curriculum study was associated with lower leisure time.
- Higher leisure usage corresponded with lower total productive study.
- Sleep showed a weaker trade-off with either productivity or leisure.

This suggests that leisure is typically reduced to make room for study during exams.

**4. Focus and Efficiency Under Exam Pressure**  
A Focus Ratio metric (productive study / total screen engagement) was used. Focus ratios peaked during exam-heavy periods, indicating that screen engagement was more likely to be used for productive purposes rather than passive leisure.

**5. Balance Highlighted Sustainable vs Strained Days**  
A balance score (sleep + productive study − leisure) showed:
- Balanced days had moderate study and adequate sleep.
- Strained days (low balance) had very high study and low leisure and sleep.

This reveals that maximum productivity does not always align with sustainable behavior.

**Overall Conclusion:**  
Exam periods lead to intentional reallocation of time toward short-term academic performance, often at the expense of leisure and long-term learning. While study efficiency improves under pressure, sustained imbalance may carry long-term recovery costs.

**Key Takeaway:**  
> Academic performance peaks during exam periods are driven more by focus and reduced leisure than by extended screen hours alone.

---

## ⚠️ Limitations
- Dataset represents a single individual and may not generalize broadly.
- November is an exam-heavy month, introducing seasonal bias.
- Data is self-reported and subject to measurement error.
- Academic performance outcomes (e.g., exam scores) were not included.
- Analysis performed as a learning project while developing data analytics skills

---

## 🚀 Future Improvements
- Compare exam months with non-exam months
- Introduce mood, energy, or focus ratings
- Automate data collection
- Expand dataset to multiple participants
- Build an interactive dashboard using Tableau, Power BI, or Streamlit

---

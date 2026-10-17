# Hospital Appointment No-Show Analysis

## Project Overview

This project analyzes a synthetic dataset of 600 hospital appointments to understand patterns in patient attendance and missed appointments. Using Python, NumPy, Pandas, and Matplotlib, the analysis explores no-show rates across hospital departments, SMS reminder groups, waiting times, and patient ages.

The goal is to demonstrate how data analysis can identify patterns and support data-informed operational decisions.

## Business Objectives

- Calculate the overall appointment attendance and no-show rates.
- Identify departments with higher and lower no-show rates.
- Compare no-show rates between SMS reminder groups.
- Examine average waiting time and patient age by attendance status.
- Present findings through charts and summary statistics.

## Tools and Technologies

- **Python** — data analysis
- **NumPy** — numerical operations and statistical calculations
- **Pandas** — data cleaning, grouping, and analysis
- **Matplotlib** — data visualization
- **Google Colab** — development environment

## Dataset

The dataset contains **600 synthetic hospital appointment records** with fields including patient age, gender, department, appointment date, scheduled date, appointment type, SMS reminder status, and attendance status.

**Data note:** This is a practice dataset, not real hospital data. The findings are illustrative and should not be generalized to actual hospitals.

## Data Cleaning and Preparation

- Inspected the dataset structure and missing values.
- Checked for duplicate records.
- Filled missing patient ages with the median.
- Replaced missing categorical values with `Unknown`.
- Converted appointment and scheduled dates into datetime format.
- Created a `Waiting_Days` feature to measure the interval between scheduling and the appointment.

## Key Findings

### Overall Attendance

- Total appointments: **600**
- Attended appointments: **476**
- No-show appointments: **124**
- Attendance rate: **79.33%**
- Overall no-show rate: **20.67%**

### Department Analysis

- **Cardiology:** Highest no-show rate at **31.88%**.
- **Pediatrics:** Lowest no-show rate at **17.58%**.
- General Medicine recorded the highest number of missed appointments, with **38 no-shows**.

### SMS Reminder Analysis

- SMS status `Yes`: **20.58%** no-show rate.
- SMS status `No`: **18.92%** no-show rate.
- SMS status `Unknown`: **33.33%** no-show rate.

The reminder groups show different no-show rates, but this descriptive analysis does not establish whether reminders caused any difference.

### Waiting-Time Analysis

- Attended appointments: average waiting time of **12.49 days**.
- No-show appointments: average waiting time of **15.28 days**.

Patients who missed appointments had a longer average waiting time in this dataset. This is an observed association, not proof of causation.

### Patient Age Analysis

- Attended appointments: average age of **51.93 years**.
- No-show appointments: average age of **52.59 years**.

The average ages were similar across the two attendance groups.

## Visualizations

The project includes charts for:

- No-show rate by hospital department.
- No-show rate by SMS reminder status.
- Average waiting time by attendance status.
- Average patient age by attendance status.

## Business Recommendations

Based on these illustrative findings, a hospital could consider:

1. Investigating appointment scheduling and attendance patterns in Cardiology.
2. Testing different reminder timings and channels before evaluating reminder effectiveness.
3. Reviewing long waiting periods and exploring ways to offer earlier appointment slots.
4. Monitoring no-show rates by department and attendance-related factors over time.

These recommendations would need validation using real hospital data before implementation.

## Conclusion

This project demonstrates a basic data analysis workflow, from data cleaning and feature engineering to KPI calculation, group-based analysis, visualization, and business recommendations. It highlights how Python libraries can help summarize appointment attendance patterns in a structured and understandable way.

## Skills Demonstrated

`Python` · `NumPy` · `Pandas` · `Matplotlib` · `Data Cleaning` · `Exploratory Data Analysis` · `KPI Analysis` · `Data Visualization` · `Business Insights`

## Disclaimer

All records are synthetic and intended for educational and portfolio purposes only. No real patient information is used.

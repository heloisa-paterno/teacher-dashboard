# Student Performance Analytics Dashboard for Teachers: Looker Studio BI Project

## Goals
Present and analyse behavioural and academic data from multiple students and classes.

Determine students who are at risk of low performance.

Investigate whether homework completion predicts improvement.

Compare performance across classes.

Evaluate behavioural indicators and their correlation with test outcomes.


## Tools
Looker Studio: Dashboard creation

Google Sheets: Data storage, preprocessing, data cleaning

Python: Text preprocessing and sentiment analysis [coming soon]


## Dataset

Fictional sample dataset based on anonymised real-world records. 

Contains year-round student data across multiple classes, including 
* Homework completion records (daily or weekly)
* Test scores and makeup test scores
* Written teacher comments throughout the year
* Multiple classes within the same grade level

### Data Model
The project uses structured tables containing:

* Students → student_id, class, grade_level
* Homework → student_id, date, completion flag
* Assessments → test_score, makeup_score, improvement flag
* Comments → comment_text

Derived metrics include:

* Homework completion rate
* Best Score (between initial and makeup testing)
* Improvement rate
* Score difference
* Risk indicator


## Features
* Filters by class/year
* Visualizations of main KPIs
* Retention, engagement, and performance metrics.


## KPIs
* Homework completion rate
* Average test score
* Improvement rate after makeup tests
* Class-level performance ranking
* Evolution throughout time


## Dashboard Pages

1. **Executive Overview**

Class comparison charts

KPI summary cards

Filters by grade and class


2. **Improvement Analysis**

Assessment-level average improvement table

Class improvement comparison

Score improvement throughout time


3. **Behaviour and Performance Analysis**

Homework completion trends

Correlation between homework and scores

Filters by grade, class and date


4. **Student-level Analysis**

Individual student selection

Student-level KPIs and trends

Targeted teacher comments


5. **Ranks**

Top students by grades and homework engagement 

Most at-risk students by grades and homework engagement 

Filters by grade and class 


6. **Qualitative Insights [coming soon]**

Teacher comments table

Sentiment analysis vs performance


## Insights

Example insights brought by the dashboard:

- Students with homework completion below 60% showed significantly lower improvement rates.
- Certain classes had consistently higher engagement but similar test averages, suggesting inherent differences in class culture.
- Certain students are at-risk when it comes to engagement but not scores.
- Homework completion correlates highly to test performance, but in-class behavioural issues (as raised in teachers' comments) do not predict performance
- High homework engagement and low test performances indicate students needing intervention


## How to run 
Copy dataset template from `/data`

Upload to Google Sheets

Replace dataset with your own

Duplicate the dashboard template in Looker Studio

Connect your data


## Dashboard
https://lookerstudio.google.com/reporting/62f2a4b5-549f-46e2-8d05-061b2de67878

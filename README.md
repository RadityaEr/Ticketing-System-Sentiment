# Ticket System Review Analysis
This is my personal project to learn how to Analyze a Dataset and build a dashboard in Power BI. The [Dataset](https://drive.google.com/file/d/1oB1j3_V3fx-M-1u_9UVrpr29719EMqu3/view) consists of various tables with the following is the one that I will use for the project:

The data preprocessing steps are done in python using [Google Colab](https://drive.google.com/file/d/1tWuGLPzdpgvW2BRafyGzwwhjj_JkntG6/view). 
Unfortunately, I don't have any Microsoft organization account so I can only export my [Dashboard](https://drive.google.com/file/d/1xaCnD-5RNqx9mQRNFwEe2oHY4k6hjtCZ/view) into a PDF file, which is also embedded in this repository


This repository contains an analysis of a Ticket System Review dataset, which is based on a survey conducted among customers using various ticketing platforms, including:

- Zendesk
- Zoho Desk
- Freshdesk
- ServiceNow
- Jira Service Management
- OTRS
## Data Understanding 
Each survey response contains the following details:
- `Survey ID & Date` : A unique identifier for each survey, along with the date it was conducted.
- `Ticket System` : The specific platform being evaluated.
- `Ratings (1-5 Scale)` : Includes ratings for overall experience, customer service, features, value for money, and ease of use.
- `Likelihood to Recommend (NPS, 0-10 Scale)` : A metric used to assess customer loyalty.
- `Customer Reviews` : Text-based feedback from users.

## Objective
The goal of this analysis is to evaluate customer feedback across different platforms by examining key metrics such as:

- Net Promoter Score (NPS)
- Overall Customer Satisfaction
- Feature-Specific Satisfaction Scores
- Customer Effort Value
- Sentiment Analysis

## Contents
Data Cleaning & Preprocessing: Handling missing values, duplicates, and outliers.

Exploratory Data Analysis (EDA): Identifying trends, distributions, and key insights.

Sentiment Analysis: Analyzing customer sentiment using text analysis techniques.

# Sentiment Analysis Approach
This project employs sentiment analysis using the Twitter RoBERTa model from Hugging Face, a state-of-the-art transformer-based model trained specifically to detect sentiment in text, particularly from social platforms like Twitter.

## Methodology
### Text Classification: The model categorizes text into three sentiment labels:

`Negative` → LABEL_0

`Neutral` → LABEL_1

`Positive` → LABEL_2
Data Processing & Analysis:

- Applied basic data cleaning (removing noise, handling missing values).
- Utilized the Transformers library to process and classify sentiment.
- Stored sentiment analysis results in two columns:
- sentiment_score → Model's confidence score for each sentiment.
- sentiment → Final sentiment label assigned to each text entry.
  
End-to-End Implementation:

From data preprocessing to sentiment classification, this project integrates machine learning models and key Python libraries, including:

Pandas → Data manipulation and structuring.

Transformers → Hugging Face library for Natural Language Processing (NLP).

This approach enhances the analysis by providing deeper insights into customer sentiment across various ticketing platforms.

Visualization & Insights: Dashboards and reports to present findings.
![Ticket_System_Customer Sentiment Dashboard_page-0001](https://github.com/user-attachments/assets/8f764924-55b2-4911-b048-2c58afcc49a1)

![Ticket_System_Customer Sentiment Dashboard_page-0002](https://github.com/user-attachments/assets/d5c908e8-0832-405e-85e0-c64f4a8dc413)



Tools Used
- Python (Pandas, NumPy, Seaborn, Matplotlib, NLP libraries)
- SQL for data querying and manipulation
- Power BI / Tableau for dashboards
  
This project provides actionable insights into customer experience, helping businesses optimize their ticketing platforms.

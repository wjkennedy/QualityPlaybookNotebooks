# Software Quality Metrics Framework - Version 0

## Introduction
This project aims to develop a framework for measuring software quality metrics and their corresponding controls in Jira. The notebooks are structured into multiple levels (Level 0-4), each representing a different stage of data processing and analysis. The levels are inspired by NASA, NEON, or NIST data product standards.

## Notebooks

### Level 0 - Raw Data Collection
- Focuses on collecting raw data from sources like GitHub and Jira.
- Utilizes Smart Commits and service account API keys.

## Level 1 - Data Cleaning

- Cleans the raw data from Level 0.
- Identifies the Primary Key and normalizes date formats for time-series analysis.

## Level 2 - Data Joining and Customer Feedback

- Joins the cleaned data with additional sources.
- Incorporates customer feedback from Amplitude, Qualtrics, and Call Miner.

## Level 3 - Advanced Analysis

- Includes statistical models, machine learning algorithms, and predictive analytics.
- Provides insights and recommendations based on the analysis.

## Gaps and Areas for Improvement

- Real Data Collection: The current version uses simulated data. The following areas need real data:
- GitHub and Jira Smart Commits (Level 0).
- Customer feedback from Amplitude, Qualtrics, and Call Miner (Level 2).
- API Integration: Integration with Amplitude, Call Miner, and Qualtrics APIs for data collection (Level 2).
- Model Implementation: The statistical and machine learning models in Level 3 are outlined in pseudocode and need to be implemented with real data.
- Authentication: The notebooks are designed to use OAuth 1.0 to connect to Jira, but the connection details need to be finalized.

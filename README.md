# Software Quality Metrics Framework - Version 0

## Introduction
This project aims to develop a framework for measuring software quality metrics and their corresponding controls in Jira. The notebooks are structured into multiple levels (Level 0-4), each representing a different stage of data processing and analysis. The levels are inspired by NASA, NEON, or NIST data product standards.

It answers 5-Hows related to Software Quality in order to assess the available metrics and aid discovery.

A 5-How analysis is a method used to explore the cause-and-effect relationships underlying a particular problem. It's a questioning technique used to explore the details of a particular issue or challenge, and it can be applied to understand the path to implementation for quality measures related to Customer Satisfaction and Service Level Agreements.

## Measures


This table provides a high-level overview of each metric, along with how it might relate to CSAT and the Bug SLA, and how it could be implemented in Jira. The actual relationships and implementations can depend on many factors and might need to be analyzed in more detail.

| Metric | Description | Relationship with CSAT | Relationship with Bug SLA | Jira Implementation |
| --- | --- | --- | --- | --- |
| Operational Measures | Monitor computer utilization, downtime, and response time. | Not directly related to CSAT. | Not directly related to Bug SLA. | System monitoring tools and Jira Service Management for incident management. |
| Ongoing Project Measures | Monthly status reports on milestones or planned vs. actual expenditures. | Not directly related to CSAT. | Can help meet Bug SLA by tracking project progress. | Jira Software with issues representing milestones and custom fields for expenditures. |
| Production Library and Backlog Measures | Full production library and backlog study. | Not directly related to CSAT. | Can help meet Bug SLA by managing the product backlog. | Jira Software for backlog management and version control systems for the production library. |
| User Satisfaction Measures | Measurement of user satisfaction. | Directly related to CSAT. | Meeting the Bug SLA can lead to higher CSAT. | Jira Service Management for CSAT surveys and user interviews. |
| Completed Project Measures | Counting the function point totals of completed projects and accumulating resource data. | Not directly related to CSAT. | Can help meet Bug SLA by tracking completed projects. | Jira Software for tracking completed issues and projects, and plugins like Advanced Roadmaps for function point analysis. |
| Soft-Factor Measures | In-depth survey of all the soft factors that influence software projects. | Can indirectly affect CSAT by improving software development processes. | Can help meet Bug SLA by improving software development processes. | Combination of tools, including Jira for tracking tool usage, and possibly surveys or other data collection methods for other factors. |
| Software Defect Measures | Measurement of software defect rates. | There is a strong observed correlation between defect levels and user satisfaction. | Can help meet Bug SLA by tracking and reducing defect rates. | Jira Software for tracking defects, and plugins like Jira Misc Workflow Extensions for calculating defect rates. |
| Enterprise Demographic Measures | Annual demographic surveys of employees in relevant skill classes. | Can indirectly affect CSAT by improving workforce planning. | Not directly related to Bug SLA. | Likely requires a separate HR system, though some information could be gathered from Jira user profiles. |
| Enterprise Opinion Survey | Survey of employee opinions. | Can indirectly affect CSAT by improving employee satisfaction. | Not directly related to Bug SLA. | Likely requires a separate survey tool, though Jira Service Management could be used for gathering some feedback. |
| Defect Escape Rate (DER) | The percentage of defects that have escaped into production compared to the total number of defects found. | High DER might lead to lower CSAT as more defects are reaching the customer. | High DER might indicate that the SLA for bug detection is not being met. | Jira Software for tracking defects and calculating DER. |
| Mean Time to Acknowledge (MTTA) | The average time it takes for a team to acknowledge that a bug or issue has been reported. | Faster MTTA can lead to higher CSAT as customers see their issues being acknowledged quickly. | MTTA is often a part of the Bug SLA, so meeting the MTTA target helps meet the SLA. | Jira Software for tracking issue creation and acknowledgement times. |
| Mean Time to Resolution (MTTR) | The average time it takes for a team to resolve a bug or issue after it has been reported. | Faster MTTR can lead to higher CSAT as issues are resolved quickly. | MTTR is often a part of the Bug SLA, so meeting the MTTR target helps meet the SLA. | Jira Software for tracking issue creation and resolution times. |
| Mean Time Between Failures (MTBF) | The average time between the occurrence of one failure and the occurrence of the next failure. | Higher MTBF can lead to higher CSAT as it indicates more reliable software. | MTBF might not directly relate to the Bug SLA, but it can indicate the effectiveness of the bug resolution process. | Jira Software for tracking issue resolution times. |
| Customer Satisfaction Score (CSAT) | A measure of customer satisfaction with a product or service. | CSAT is the metric being optimized. | Meeting the Bug SLA can lead to higher CSAT. | Jira Service Management for CSAT surveys. |
| Bug SLA Compliance Rate | The percentage of bugs for which the SLA was met. | Higher SLA compliance can lead to higher CSAT as it indicates that issues are being resolved in a timely manner. | This is a measure of how well the team is meeting the Bug SLA. | Jira Service Management for tracking SLA compliance. |
| Defect Removal Efficiency (DRE) | The percentage of defects that are caught during the testing phase as opposed to being found in production. | Higher DRE can lead to higher CSAT as it indicates that fewer defects are reaching the customer. | Higher DRE might indicate that the SLA for bug detection is being met. | Jira Software for tracking defects and calculating DRE. |

----


### 1. Operational Measures
**How can we monitor computer utilization, downtime, and response time?**
1. How do we identify the key performance indicators (KPIs) for system operation?
2. How do we collect data on these KPIs?
3. How do we analyze this data to detect anomalies or trends?
4. How do we integrate this analysis into our incident management process?
5. How do we ensure that the incident management process leads to effective resolution and continuous improvement?

### 2. Ongoing Project Measures
**How can we provide monthly status reports on milestones or planned vs. actual expenditures?**
1. How do we define the milestones and expenditure targets for each project?
2. How do we track progress towards these milestones and expenditures?
3. How do we collect and consolidate this data across multiple projects?
4. How do we present this data in a meaningful way to stakeholders?
5. How do we use this information to make informed decisions and improve project management?

### 3. Software Defect Measures
**How can we measure software defect rates?**
1. How do we define what constitutes a defect in our software?
2. How do we detect and record these defects?
3. How do we categorize and prioritize these defects?
4. How do we analyze defect trends over time?
5. How do we use this analysis to improve software quality and reduce defect rates?

### 4. Mean Time to Resolution (MTTR)
**How can we measure the average time it takes for a team to resolve a bug or issue?**
1. How do we define what constitutes resolution for different types of issues?
2. How do we track the time from issue reporting to resolution?
3. How do we analyze this data to calculate the average time to resolution?
4. How do we present this information to the team and stakeholders?
5. How do we use this information to improve resolution processes and meet SLAs?

### 5. Customer Satisfaction Score (CSAT)
**How can we measure customer satisfaction with a product or service?**
1. How do we define what constitutes customer satisfaction for our products or services?
2. How do we collect feedback from customers on their satisfaction levels?
3. How do we analyze this feedback to calculate a CSAT score?
4. How do we present this information to the team and stakeholders?
5. How do we use this information to improve customer satisfaction?

By asking these "How" questions, we can delve into the underlying processes and dependencies for each metric. This approach allows us to understand the path to implementation without assuming any particular tools, and it can be adapted to the specific needs and context of your organization.

----


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

# Clustering Student Profiles for Scaler (Industry : EdTech)
This project explores Scaler’s learner database to analyze how career trajectories, job profiles, and compensation patterns vary across different companies and experience levels.


# Project Overview
This project examines Scaler’s learner data to uncover how earning potential and career progression vary across job profiles, companies, and experience levels. It aims to answer key questions such as: Which job roles command the highest salaries? How does experience correlate with compensation? The insights derived can help Scaler refine its curriculum and offer targeted career counseling for better learner outcomes.

# Problem Statement
As a data scientist within the analytics vertical of this leading EdTech platform, the task is to analyze and cluster learners based on their job profiles, companies, and related features. The objective is to derive meaningful clusters that reflect shared characteristics among learners, enabling deeper insights into employment trends, company segments, and learner career progression.

# Objectives
  - Perform Exploratory Data Analysis (EDA) to understand the dataset and clean it for processing.
  - Cluster learners based on attributes like current job profiles, employment start year, CTC details, and company identifiers.
  - Generate actionable insights and recommendations by profiling companies, positions, and salary distributions, and highlighting top/bottom performers.
  - Utilize manual and unsupervised clustering techniques to create meaningful groupings and analyze their implications.

# Data Set
  - Unnamed 0: Index of the dataset
  - Email_hash: Anonymised Personal Identifiable Information (PII)
  - Company_hash: Anonymized identifier for the company, which is the current employer of the learner
  - orgyear: Employment start date
  - CTC: Current CTC
  - Job_position: Job profile in the company
  - CTC_updated_year: Year in which CTC got updated (Yearly increments, Promotions)

# Milestones
  - Exploratory Data Analysis (EDA): Statistical summary, handling missing values, removing duplicates, and cleaning text with regex.
  - Feature Engineering: Creating new features like years of experience and generating flags (Designation, Class, Tier) for manual clustering.
  - Manual Clustering: Analyzing learner performance and categorizing based on company, job position, years of experience, and salary distribution.
  - Unsupervised Learning: K-means clustering (determining optimal clusters using the elbow method) and Hierarchical clustering.
  - Insights and Recommendations: Profiling top/bottom employees and companies, identifying key trends, and providing strategic recommendations.

# Findings
  - There are 41,216 duplicate entries where a single email_hash appears more than once, indicating learners may have multiple records for different roles or companies.
  - The most frequent job position is "Backend Engineer" accounting for a significant portion of the dataset.
  - Employees identified in Tier 1 have significantly higher CTC than their company's average, likely holding critical roles.
  - Data Science professionals in Class 1 are earning above the average CTC of their peers within the same job position and company.
  - Employees with mid-level experience (5-7 years) earning more than their peers are likely in managerial or specialized technical roles.
  - Hopkins Statistic of 0.961 suggests there is a strong tendency for clustering.
  - The optimal number of clusters (k) for K-Means was determined to be 4 using the Elbow Method and Silhouette Score.
  - Cluster 0 (26.4%): Represents relatively tenured employees (median orgyear 2016) with moderate CTC levels, indicating a higher hierarchy in the organization.
  - Cluster 1 (18.7%): Represents relatively newer employees (median orgyear 2018) with moderate CTC levels and lower hierarchy.
  - Cluster 2 (16.0%): Represents highly experienced employees (median 17 years) in leadership roles earning competitive CTCs.
  - Cluster 3 (39.0%): The largest cluster, representing moderately experienced employees (median 10 years) with lower-tier designations and compensation.
  - Hierarchical clustering (dendrogram) visually suggests three distinct broad clusters.
  - Tier 3 learners are predominantly associated with relatively lower-paying job positions and companies with less competitive compensation structures

# Recommendations
  - Develop targeted upskilling programs for Tier 3 learners focusing on high-demand job roles and premium-paying skills.
  - Partner with premium companies to create mentorship programs that facilitate transition to Tier 1 roles.
  - Encourage re-evaluation of compensation structures for companies with anomalous compensation practices to align with industry standards.
  - Offer certifications and courses in niche technologies and tools for entry-level learners to justify high market demand and higher CTCs.
  - Focus on leadership and strategic management courses for learners targeting Engineering Leadership roles.
  - Update QA and Frontend Engineer curricula to include advanced tools and technologies to increase earning potential.
  - Provide personalized career counseling based on cluster characteristics, focusing on career advancement and strategic transitions for low-earning clusters.

# Colab Link
  - https://colab.research.google.com/drive/1GRT9Kq8-4-XEFEtE4lT3sjt3lKQZzqYy

# Data Link
  - https://drive.google.com/file/d/1FcH3qusAKgmSZ_SWA-C9A-4mlzP7nQ00/view?usp=drive_link

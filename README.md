TikTok Video Engagement — Exploratory Data Analysis

Overview

This project explores an educational TikTok dataset provided through Google/Coursera coursework. The analysis investigates which characteristics and engagement patterns distinguish videos labeled as claims from videos labeled as opinions.

The original analysis began as a Coursera lab. I reorganized it into a portfolio case study and extended it with an independent analysis of normalized engagement rates.

Business Question

Which characteristics and engagement patterns appear to distinguish claim videos from opinion videos?

Dataset

19,382 records

12 original variables

Video duration and transcription

Verification and author-ban status

Views, likes, shares, downloads, and comments

Target variable: claim_status

The dataset is educational course material and should not be interpreted as internal or production TikTok data.

Tools

Python

Pandas

NumPy

Matplotlib

Jupyter Notebook

Analysis

The notebook covers:

Data inspection and missing-value checks

Descriptive statistics

Distribution analysis

Outlier detection using a modified IQR threshold

Claim vs. opinion engagement

Verification and author-ban status

Views vs. likes relationship

Independent engagement-rate feature engineering

Key Findings

Claim videos had approximately 501,555 median views, compared with 4,953 for opinion videos.

Claim videos had roughly 101× the median view count of opinion videos.

Claim videos accounted for approximately 99% of total views among labeled records.

About 31.7% of claim-video authors were banned or under review, compared with about 7.0% of opinion-video authors.

Engagement metrics were strongly right-skewed and contained many high-value observations consistent with viral-content behavior.

After normalizing engagement by views, claim videos still had higher median like and share rates.

Repository Structure

tiktok-eda-analysis/
├── README.md
├── tiktok_eda_analysis.ipynb
├── requirements.txt
└── data/
    └── README.md

How to Run

Clone or download the repository.

Place tiktok_dataset.csv inside the data/ folder.

Install the required packages:

pip install -r requirements.txt

Open tiktok_eda_analysis.ipynb in Jupyter Notebook or JupyterLab.

Run all cells.

Next Steps

A logical continuation would be to build a classification model that predicts claim_status and evaluate whether view count, author status, raw engagement metrics, and normalized engagement-rate features remain predictive when considered together.

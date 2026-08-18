# TikTok Exploratory Data Analysis

## Overview

Exploratory data analysis of 19,382 TikTok videos to investigate
differences between videos containing claims and videos expressing
opinions.

## Business Question

What characteristics and engagement patterns distinguish claim videos
from opinion videos?

## Tools

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Analysis

- Data quality and missing values
- Descriptive statistics
- Distribution analysis
- Outlier detection using IQR
- Claim vs opinion engagement
- Account verification and ban status
- Relationships between views, likes, shares, comments and downloads

## Key Findings

- Claim videos had a median of ~501K views compared with ~5K for
  opinion videos.
- Claim videos generated approximately 99% of total views.
- Authors posting claims were substantially more likely to be banned
  or under review.
- Engagement variables were heavily right-skewed and contained many
  high-value observations consistent with viral content.

## Conclusion

Video engagement, particularly view count, appears to strongly
differentiate claim videos from opinion videos. Account status may
also provide useful predictive information for a future classification
model.

# Classifying-Post-Engagement-on-Social-Platforms

A Data Science Project for Multiclass Classification Based on Social Media Post Performance
Project Overview
This project aims to predict the engagement level (Low, Medium, or High) of social media posts based on their content characteristics and performance metrics. Using a dataset of posts across platforms like TikTok, YouTube, Instagram, and Twitter, we explore how variables such as platform, content type, hashtag, region, views, likes, shares, and comments influence engagement outcomes.

By building a multiclass classification model, this project simulates a tool that could help marketing and content teams forecast the success of a post before it's published, enabling more informed decisions and higher-performing content strategies.

Business Problem
Marketing teams often struggle to predict which types of content will drive the highest engagement on social media. This project addresses that gap by using historical data to model engagement levels and identify the features that most strongly influence post performance.

Tools & Technologies
Python (Pandas, NumPy, Seaborn, Matplotlib)
Scikit-learn for modeling and evaluation
XGBoost / Random Forest (optional)
Jupyter Notebook for analysis
Git/GitHub for version control and collaboration

Exploratory Data Analysis (EDA)
The EDA revealed:

Engagement metrics (likes, comments, shares) are distributed differently across content types.
Comments appear to be a stronger signal of overall engagement than views or shares alone.
Categorical features like Platform, Content_Type, and Region show diverse performance patterns, suggesting that no single feature fully explains engagement levels.
These findings support the need for a multivariate classification model and motivate the creation of new engineered features.

Feature Engineering
To improve model performance, we apply several preprocessing steps:

One-hot encoding for categorical features (Platform, Region, Content_Type, Hashtag)
New features like:

likes_per_view
comments_per_view
shares_per_view
total_interactions (sum of likes, shares, comments)

Scaling of numeric values to handle feature range differences
Balancing classes if needed using techniques like SMOTE or class weighting

Modeling Approach
We train and evaluate multiple classification models, including:

Logistic Regression
Random Forest
XGBoost (if applicable)

Models are evaluated using:

Accuracy
F1 Score (macro/micro)
Confusion Matrix
Feature Importance Analysis

Success Criteria
A successful model will:

Achieve strong F1 scores across all three engagement levels (not just the majority class)
Highlight meaningful feature relationships
Offer actionable insights for content and marketing teams to improve engagement

Key Takeaways
Predicting engagement levels is possible using a combination of metadata and engagement metrics.
Engineered features like interaction rates significantly improve model understanding.
Insights from this project could help companies optimize posting strategies and content types by platform and region.

Project Structure
.
├── data/
│   └── raw_social_media_dataset.csv
├── notebooks/
│   └── 01_EDA.ipynb
│   └── 02_Preprocessing_and_Modeling.ipynb
├── visuals/
│   └── kde_views_by_content.png
├── README.md
└── requirements.txt

Next Steps
Tune model hyperparameters for optimal performance
Explore time-based features (if timestamps are available)
Deploy as a simple web tool or dashboard for content teams

🙋‍♀️ Author
Lupe Covarrubias
Aspiring Data Scientist | Background in Biological Engineering


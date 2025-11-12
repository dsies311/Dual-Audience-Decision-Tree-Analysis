# Dual-Audience-Decision-Tree-Analysis
Dual-Audience Decision Tree Analysis

Author: Dylan Siesky
Course: Module 10 – Decision Trees and Tree-Based Models
University of Richmond

Project Overview

This project demonstrates the ability to build, evaluate, and communicate the results of machine learning models to two different audiences: technical stakeholders and non-technical business leaders. The analysis uses decision tree models to predict whether a company’s stock from the S&P 500 will close higher or lower on June 30, 2025, based on its trading activity from the two prior days.

The notebook showcases both technical implementation (model training, evaluation, and visualization) and business translation (simplified findings and actionable insights), reflecting the real-world role of data analysts as both modelers and communicators.


Objectives

Develop predictive models using Decision Tree Classifiers with varying depths to explore the impact of model complexity on performance.

Evaluate performance through training and testing accuracy, confusion matrices, and visualizations of tree structure and feature importance.

Communicate insights effectively to both technical and non-technical audiences, balancing statistical rigor with clarity and accessibility.


Dataset

The dataset contains daily trading data for 503 companies in the S&P 500 from January through June 2025. Each record includes opening price, closing price, and trading volume for each trading day. The target variable (price_up) indicates whether a company’s stock price increased on June 30, 2025, compared to its opening price. Predictor features are derived from the two previous trading days (June 26 and June 27).


Notebook Structure

Section 1 – Technical Analysis & Code
Includes data preparation, feature engineering, and creation of the price_up target. Three decision tree models were trained using max_depth = 3, 5, 10 and evaluated with accuracy scores, confusion matrices, and visualizations.

Section 2 – Technical Stakeholder Report
Written for data scientists and analytics managers. Describes the methodology, overfitting analysis, model comparison, and the rationale for selecting the optimal tree depth.

Section 3 – Non-Technical Stakeholder Report
Written for business executives and portfolio managers. Summarizes results in plain language, highlighting short-term trends, key predictors, and real-world implications without technical jargon.

Section 4 – Reflection
A two-paragraph reflection discussing the challenges of translating technical information for non-technical audiences and the importance of clear, adaptive communication.


Key Takeaways

A medium-depth decision tree (max_depth = 5) provided the best balance between interpretability and performance.

Short-term stock momentum and trading volume were the strongest predictors of next-day movement.

The model achieved approximately 65–70% accuracy, but this reflects pattern recognition within the dataset, not a guaranteed or profitable trading strategy.

Effective data communication depends on presenting insights that align with the audience’s level of technical understanding and decision-making needs.


Technologies Used

Python: pandas, numpy, scikit-learn, matplotlib

Environment: Google Colab / Jupyter Notebook

Version Control: GitHub


How to Run the Notebook

Upload sp500_2025_h1.csv to your Google Drive.

In Google Colab, mount your Drive:
from google.colab import drive
drive.mount('/content/drive')

Update the file path in the notebook if needed (default: /content/drive/MyDrive/sp500_2025_h1.csv).

Run all cells in order from top to bottom.

Review the printed accuracy scores, confusion matrices, and visualizations.

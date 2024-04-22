# Railway Anomaly Detection and Feature Comparison

This repository contains code for a data analysis project focused on anomaly detection and feature comparison in railway operations data. The project includes Exploratory Data Analysis (EDA), data preparation, Principal Component Analysis (PCA), and outlier detection using machine learning techniques.

## Overview

Railway operations data often contain anomalies that can impact efficiency and safety. This project aims to identify and analyze outliers within railway data, as well as compare features between outlier and non-outlier instances to uncover patterns and insights.

## Key Components

### 1. Exploratory Data Analysis (EDA)

- Perform initial exploration of the dataset (`df_march_2024`).
- Identify and handle missing values, outliers, and data quality issues.
- Derive new features from the `timeTableRows` column to enrich the dataset.

### 2. Data Preparation

- Encode categorical features using one-hot encoding for machine learning compatibility.
- Prepare the dataset (`df_encoded`) for dimensionality reduction and outlier detection.

### 3. Principal Component Analysis (PCA)

- Standardize the preprocessed data.
- Apply PCA to reduce the dimensionality of the dataset while preserving variance.
- Determine the optimal number of principal components to capture a desired variance threshold (e.g., 95%).

### 4. Outlier Detection

- Utilize Isolation Forest, a machine learning algorithm, to detect outliers in the PCA-transformed feature space.
- Assign anomaly scores (`-1` for outliers, `1` for inliers) and identify outlier instances.

### 5. Feature Comparison and Statistical Analysis

- Compare categorical features (e.g., `trainCategory`, `trainType`) between outliers and non-outliers.
- Conduct statistical tests (e.g., Chi-squared test, T-test, Z-test) to quantify differences in feature distributions.
- Visualize feature comparisons using bar plots to highlight distinctions.

## Usage

### Requirements

- Python 3.x
- Jupyter Notebook or any IDE supporting Python

### Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/sgbyteninja/finnland_trains_anomaly_detection
   cd railway-anomaly-detection

# Student Performance Prediction Analysis

## Overview
This project analyzes student performance using different feature selection methods and machine learning models. It uses a dataset containing information about students' study hours, socioeconomic scores, sleep hours, and attendance percentages to predict their grades.

## Features
- Study Hours
- Socioeconomic Score
- Sleep Hours
- Attendance (%)

## Methods Used

### Feature Selection Methods:
1. **Gini Importance**
   - Based on Random Forest algorithm
   - Shows Study Hours (73.9%) and Socioeconomic Score (25%) as most important

2. **Mutual Information**
   - Information theory based selection
   - Confirms Study Hours (80.4%) as the dominant feature

3. **Firefly Algorithm**
   - Nature-inspired optimization
   - Selected all features as relevant

### Prediction Models:
1. **Random Forest**
   - Best performing model
   - R² Score: 0.98 (98% accuracy)
   - MSE: ~1.45

2. **Support Vector Machine (SVM)**
   - Lower performance compared to Random Forest
   - R² Score: 0.91 (91% accuracy)
   - MSE: ~6.98

## Key Findings
1. Study Hours is the most influential factor in predicting grades
2. Random Forest consistently outperforms SVM across all feature selection methods
3. All feature selection methods yield similar model performance

## Dependencies
```python
pandas
numpy
scikit-learn
matplotlib
```

## Usage
1. Prepare your data in CSV format with columns for study hours, socioeconomic score, sleep hours, attendance, and grades
2. Run the main script
3. View the visualizations and performance metrics

## Visualizations
The code generates two main plots:
1. Feature importance comparison across selection methods
2. Model performance comparison (R² Score and MSE) for different feature selections

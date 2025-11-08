# Student Purchase Prediction

## Project Overview
This project predicts whether a free-plan student will purchase a subscription on the 365 platform based on their activity (lecture views, exams, etc.). It explores preprocessing, feature engineering, and machine learning modeling.

## Data
The dataset contains 7 predictor variables and 1 target variable (`purchased`). Features include:
- `days_on_platform`
- `minutes_watched`
- `courses_started`
- `practice_exams_started`
- `practice_exams_passed`
- `minutes_spent_on_exams`
- `student_country`

## Models
- Logistic Regression
- K-Nearest Neighbors (GridSearchCV)
- Support Vector Machine (GridSearchCV + scaling)
- Decision Tree (with pruning via `ccp_alpha`)
- Random Forest

## Key Steps
1. Data cleaning and preprocessing
2. Removing outliers
3. Handling missing values
4. Multicollinearity check (VIF)
5. Encoding categorical variables
6. Train-test split
7. Model building and evaluation

## Results
- Confusion matrices, classification reports, and F1-scores were analyzed.
- Random Forest performed best for predicting students likely to purchase.

## How to Run
1. Clone the repository
2. Install requirements:
   ```bash
   pip install -r requirements.txt

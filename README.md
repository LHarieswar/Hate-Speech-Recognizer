# Hate Speech Recognizer

This project aims to detect hate speech in tweets and classify them based on sentiment analysis. It includes data preprocessing, visualization, and machine learning-based classification.

## Dataset Overview
The dataset consists of 10,575 tweets with three columns:
- **id**: Unique identifier for each tweet.
- **label**: 1 for hate speech, 0 for non-hate speech.
- **tweet**: The tweet text, with mentioned usernames replaced by `@user`.

## Preprocessing Steps
To clean and prepare the data, the following steps were performed:
- Converting text to lowercase.
- Removing URLs and hashtags using regex.
- Eliminating punctuation.
- Tokenizing tweets and removing stop words.
- Removing duplicate entries.

## Data Visualization
To better understand the dataset, the following visualizations were generated:
- **Pie chart**: Displays the percentage of hate vs. non-hate tweets.
- **Word clouds**: Separate visualizations for hate speech and non-hate speech tweets to highlight commonly used words.

## Model Development
The dataset was split into **80% training** and **20% testing** using `train_test_split()`. Several classification models were implemented:
1. **Logistic Regression**
2. **Random Forest**
3. **Naïve Bayes**
4. **Support Vector Machine (SVM)**
5. **XGBoost**

## Results
- **XGBoost** initially achieved the highest accuracy.
- After hyperparameter tuning, **Random Forest** outperformed other models.

## Usage
The dataset (`.csv` file) and the Jupyter Notebook containing the full implementation can be found in the **ML project source code** and **data folder**.

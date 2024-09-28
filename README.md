# Machine Learning Approaches to Predict the Netflix APP Ratings

Here’s a table of contents to include in your `README.md`:

---

## Table of Contents
1. [Overview](#overview)
2. [Dataset](#dataset)
3. [Methodology](#methodology)
   - [Sample](#sample)
   - [Explore](#explore)
   - [Modify](#modify)
   - [Model](#model)
   - [Assess](#assess)
4. [Models Used](#models-used)
   - [Support Vector Machine (SVM)](#support-vector-machine-svm)
   - [Random Forest](#random-forest)
   - [XGBoost](#xgboost)
   - [Neural Network](#neural-network)
5. [Results](#results)
6. [Data Visualization](#data-visualization)
7. [Business Insights](#business-insights)
8. [Limitations](#limitations)
9. [Future Work](#future-work)


This table of contents will help users navigate your `README.md` easily.

## Overview
This project focuses on predicting Netflix user ratings from reviews posted on the Google Play Store, utilizing machine learning and natural language processing (NLP) techniques. The data spans from 2017 to 2023, capturing user sentiment before, during, and after the COVID-19 pandemic. The goal of the project is to analyze how users rate Netflix and identify key issues, enabling Netflix to enhance its services.

## Dataset
- **Source**: Google Play Store reviews for the Netflix app, sourced from Kaggle.
- **Records**: 1,121,434 records after cleaning.
- **Features**: `review_text`, `review_rating`, `likes`, `year_of_posting`.

## Methodology
The project employs the **SEMMA** (Sample, Explore, Modify, Model, Assess) methodology:
1. **Sample**: Dataset extracted from Google Play reviews, filtered from 2017-2023.
2. **Explore**: Visual analysis of review trends across years and ratings.
3. **Modify**: Preprocessing of text data, including tokenization, stop word removal, handling of emojis, and vectorization.
4. **Model**: Comparison of machine learning models (Random Forest, XGBoost, SVM, and Neural Networks) to classify user ratings.
5. **Assess**: Evaluation based on accuracy, precision, recall, and F1-score.

## Models Used
1. **Support Vector Machine (SVM)**
2. **Random Forest**
3. **XGBoost**
4. **Neural Network**

### Best Performing Model
- **Neural Network**: Achieved the highest accuracy on test data with 72.4%. It also outperformed other models on precision, recall, and F1-score.

## Results
- **Neural Network**: Best performing model with an accuracy of 72.4% on the test set.
- **Random Forest**: Showed signs of overfitting with high training accuracy (95.3%) but lower test accuracy (67.9%).
- **Data Insights**: A word cloud of low-rating comments revealed user concerns related to app updates, device compatibility, and subscription policies.

## Data Visualization
- Bar charts of review distribution across years and ratings.
- Word clouds generated from review text highlighting common sentiments across different time periods.

## Business Insights
- **Improvement Areas**: Version stability, subscription flexibility, content quality, and sensitivity to regional preferences.
- **Recommendation**: Address device compatibility, update issues, and subscription options to improve user experience.

## Limitations
- The analysis is limited to reviews from Google Play. Expanding data sources (e.g., Apple Store) could enhance reliability.
- Slang and nuanced meanings in user comments may not be fully captured by current NLP methods.

## Future Work
- Incorporating additional data sources.
- Expanding the model to analyze reviews from other social media platforms like Facebook, Twitter, and Instagram.


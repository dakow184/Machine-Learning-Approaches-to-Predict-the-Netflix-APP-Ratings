# Machine Learning Approaches to Predict the Netflix APP Ratings

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
  ![image](https://github.com/user-attachments/assets/48400a60-c071-48f9-8525-a831fa44fed5)
  
![image](https://github.com/user-attachments/assets/8744f4ab-c925-4ff4-961c-9922b67584c5)

- Word clouds generated from review text highlighting common sentiments across different time periods.

<p align="center">
  <img width="250" alt="image" src="https://github.com/user-attachments/assets/e4bc8e5e-a0f2-4f65-bba7-3347badbe2b3" style="margin: 10px;">
  <img width="400" alt="image" src="https://github.com/user-attachments/assets/059f1230-ef16-49cc-958d-8b1154517057" style="margin: 10px;">
  <img width="400" alt="image" src="https://github.com/user-attachments/assets/473fb07e-e92a-49d1-94fb-0c6bf3a8937d" style="margin: 10px;">
  <img width="400" alt="image" src="https://github.com/user-attachments/assets/57427e20-6b1f-48e2-a496-271951c89a88" style="margin: 10px;">
</p>

## Business Insights
### Improvement Areas:
1. **Version Stability**: 
   - Users reported frequent crashes after updates, indicating a need for improved testing and device compatibility.
   
2. **Subscription Flexibility**: 
   - Limited subscription options led to dissatisfaction. Offering flexible combinations of features like ads, content selection, membership sharing, and tiered pricing could better cater to user preferences.
   
3. **Content Quality**:
   - Users noted slow and outdated content updates. Delivering more frequent updates, especially in competitive regions, is key.
   
4. **Regional Sensitivity**: 
   - Cultural inaccuracies, such as in Egyptian content, resulted in backlash. Tailoring content to regional norms and values is critical.

### Recommendations:
- **Device Compatibility**:
   - Improve app testing across devices and consider lighter versions for older devices.
   
- **Subscription Plans**:
   - Offer flexible plans (e.g., weekly or family options) to better meet user needs, especially in challenging economic times.
   
- **Content Strategy**:
   - Focus on frequent content updates and partner with local creators to provide culturally relevant content.
   
- **Cultural Sensitivity**:
   - Ensure content aligns with regional norms to avoid misrepresentation and backlash. Strengthen the content review process to address cultural sensitivities more effectively.

## Limitations
- The analysis is limited to reviews from Google Play. Expanding data sources (e.g., Apple Store) could enhance reliability.
- Slang and nuanced meanings in user comments may not be fully captured by current NLP methods.

## Future Work
- Incorporating additional data sources (e.g., Apple Store reviews, official download URLs) to improve analysis reliability.
- Expanding the model to analyze reviews from other social media platforms such as Facebook, Twitter, and Instagram.
- Exploring deeper context in text meaning, especially within the framework of internet slang and evolving expressions.
- Expanding the dictionary to capture nuanced meanings and improve sentiment analysis accuracy.


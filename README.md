
# Consumer Behavior Analysis and Product Purchase Prediction in E-Commerce

## Overview
This project analyzes e-commerce user behavior and builds predictive models to forecast product purchase actions. 
The study uses a large-scale **User Behavior Dataset from Taobao (Alibaba)**, containing interactions such as clicks, 
cart additions, favorites, and purchases. The goal is to extract valuable insights, segment customers, and develop 
predictive models using deep learning.

## DataSet
used large-scale **User Behavior Dataset from Taobao (Alibaba)** From **Link:** https://tianchi.aliyun.com/dataset/649

## Pipeline
The project follows a complete pipeline:
1. **Data Preprocessing**
   - Cleaning null and duplicate records.
   - Filtering data within a valid time range.
   - Converting timestamps to datetime format and extracting time features (hour, day, weekday).
2. **Exploratory Data Analysis (EDA)**
   - Analyzing user activity trends by hour and weekday.
   - Identifying peak purchasing times and promotional event effects.
   - Investigating conversion rates across top-selling categories.
3. **Customer Segmentation**
   - Using the **RFM model (Recency, Frequency, Monetary)** to measure customer value.
   - Applying **K-means clustering** to classify users into segments such as churn-risk, loyal customers, etc.
4. **Model Development and Implementation**
   - Sequential user actions are modeled using **Recurrent Neural Networks (RNN)** and **Long Short-Term Memory (LSTM)**.
   - Models are trained and evaluated to predict the next user action.
   - Performance is compared between RNN and LSTM.

## Results
- **User Activity Trends**: Peaks observed during midday and weekends, especially around promotional events.
- **Conversion Analysis**: Conversion rates remain below 5% even for top-selling categories, highlighting a gap between browsing and purchasing.
- **Customer Segmentation**: About 60.1% of users are identified as churn-risk customers.
- **Model Performance**:
  - LSTM achieved a test accuracy of **86.3%**.
  - RNN achieved a test accuracy of **85.2%**.

## Technologies Used
- **Apache Spark** for distributed data preprocessing and analysis.
- **Python (PyTorch, Pandas, Matplotlib, Scikit-learn)** for modeling and visualization.
- **Clustering (K-means)** for customer segmentation.
- **Deep Learning (RNN, LSTM)** for sequential modeling.

## File Description
- `Consumer Behavior Analysis and Product Purchase Prediction in E-Commerce.ipynb`  
   Jupyter Notebook containing the complete pipeline, analysis, visualizations, and models.

## Future Work
- Integrating with recommendation systems to forecast product preferences.
- Incorporating contextual and demographic features (e.g., location, device, seasonality).
- Exploring advanced sequential models such as **Transformers (BERT4Rec, SASRec)**.
- Implementing real-time prediction and deployment in production e-commerce platforms.

---
**Author**: Yasser Kuhail  
**Date**: 2025  

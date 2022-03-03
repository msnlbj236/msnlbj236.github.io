---
title: "Projects"
permalink: /project/
author_profile: true
---

Research Projects 
--------------
* *Accelerating Decentralized Momentum SGD in Large-batch Deep Learning for Object Detection*
  * **Motivation**:
      <p align="center"><img width="650" height="225" src='/images/transResearch/motivation.png'></p>
      
  


* *Stochastic Optimization and Data Compression in Distributed Learning for Image Classification*
  * **Motivation**: 
 

     
Course Projects 
------------- 
* *Real-time Parking Space Detection*
  - Captured 600+ parking lots images from video with OpenCV and pre-processed images based on Grayscale Transform.
  - Applied multiple image processing methods for image augmentation, expanded train dataset size by 10 times.
  - Conducted image segmentation based on Hough Transform, Harris Corner Detector and Canny Edge Detector.
  - Performed feature detection and matching, homography estimation with MOPS descriptor, SIFT descriptor and RANSAC.
  - Built and trained CNN model based on VGG16 and MobileNet for identification using Keras, got 92.4% validation accuracy.
  - Created a real-time parking space detector to predict the available or occupied parking spots from 600+ parking lots 

* *Used Car Market Forecast* 
  - Mined and engineered 400k historical trades over 12 months for used car markets to predict the car price for future trades.
  - Performed EDA and visualized the time series and the correlation matrix of features with price using python.
  - Engineered 40 key features including Make, Model and Mileage, performed PCA to extract the usable data after encoding.
  - Predicted car price with multiple tree-based prediction models (XGBoost, LightGBM, Catboost), achieved MAE as 180.
  - Designed a fully connected Neural Networks with activation function of softplus, tuned the regressor with 5-fold cross validation and trained with iterative decreasing learning rate, reduced MAE by 26.7%.

* *News Recommendation System*
  - Developed data pipeline to clean and label 3M clicks data over 0.36M articles from MySQL database with python.
  - Calculated cosine similarity and SVD Matrix Factorization to quantify the similarity between articles.
  - Lessened recommendation list from item-based collaborative filtering (ItemCF), top-k clicking news and embedding retrieval.
  - Identified 12 key metrics for recommendation model, including news category, words count, user logs and click timestamp.
  - Trained GBDT+LR (Logistic Regression), LightGBM and DIN (Deep Interest Network) model, performed model stacking for predictions with the evaluation metric of mean reciprocal rank (MRR), achieved MRR as 0.3110.
  - Built a recommendation system to predict 5 most recommended articles based on user’s click history, targeting for 0.3M users

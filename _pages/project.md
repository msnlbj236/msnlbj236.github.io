---
title: "Projects"
permalink: /project/
author_profile: true
---

Research Projects 
--------------
* *Accelerating Decentralized Momentum SGD in Large-batch Deep Learning for Object Detection*
  * **Motivation**: Urban systems, including transporations and buildings are highly interrelated given the spatial-temporal flow of system users. The change of magnitude of occupancy in one system can be in proportion to the fluctuation in one another. In this project we aim at investigating the edge potential of predicting the energy profile of buildings, from the rich and fine-grained transportation data including realtime traffic flow intensity, and public transit status. The refined prediction would further improve the performance of Model Predictive Control (MPC) on building energy management. [link](). 

      <p align="center"><img width="650" height="225" src='/images/transResearch/motivation.png'></p>
      
  * **Modeling**: The problem is formulated as a m-to-n task, i.e., to prediction the energy profile at next n quarters using all information available up to m quarters ago. A Spatial-Temporal Graph Attention Network (STGAT) framework is proposed to capture the heterogeneous dynamic of public transit (bus) and traffic flow (inrix), where the integrated information is passed to fully-connected networks with historical energy profile and weather features to make the prediction. When compared with state-of-the-art time series baseline models, it is validated the inclusion of ambient transporation reduced the overall RMSE from 0.0478 to 0.0418.

      <p align="center"><img width="900" height="300" src='/images/transResearch/STGAT.png'></p>


* *Stochastic Optimization and Data Compression in Distributed Learning for Image Classification*
  * **Motivation**: Intelligent Transportation Systems (ITS) are critical components to strengthen travel safety, reduce congestion and improve urban mobilities. The reliability of the system depends on spatial-temporal analytics of key traffic parameters such as density, volume, and speed, which are inferred from sensors including loop detectors and cameras using computer vision. However, the former sensors suffer from high initial costs and low frequency, while the latter may deteriorate in high occlusion and large perspective cases. Thus, in this series of research we explore the effectiveness of fusing features captured by existing transportation sensors and vision-based models for traffic parameter inference. Specifically, we have leveraged domain features with convolutional neural networks to estimate vehicle density and speed (through tracking) separately. Compared with pure visual techniques, it is validated that the inclusion of domain features improves the overall performance, and we look forward to expanding the model for other transportation tasks in future.
 
  * **Detection**: To esimate the density of vehicles, we implemented a model with CNN+rLSTM module for image inputs, and LSTM module for processed transportation features including location of buses and average traffic speed. Compared with pure vision-based detection model YOLO, we have reduced the MAE from 0.73 to 0.27, and justified the effectiveness of domain features. The detailed implementation can be found [here](). 


  * **Tracking**: The speed estimation problem is tackled by tracking-by-detection framework. Basically, we have fine-tuned YOLO with self-labelled data as detector, and adopted Deepsort framework as tracker. However, we used LSTM network trained with transportation features instead of the Kalman filter as the state estimation module. In addition, the deep appearance descriptor was fine-tuned using UA-DETRAC and self-labelled data. Tested on one hour's data, it is validated that the fused model improved MOTP from 78.5% to 80.6%, and MOTA from 65.7% to 68.3% respectively. A sample result is attached below. 
  
     
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

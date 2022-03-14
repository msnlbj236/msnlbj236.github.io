---
title: "Projects"
permalink: /project/
author_profile: true
---

Research Projects in Semiconductor Optics
--------------
* *Spectroscopy and Simulation Revealed Strong Interaction of Insulating States in Moiré Superlattice*     
  -	Fabricated a WSe2/WS2 moiré Superlattice with piezo stage. Performed SHG spectroscopy to determine the crystal orientation.
  -	Implemented Microwave Impedance Microscopy to study the low conductivity at correlated insulating states.
  -	Performed PL spectroscopy to study the strong interaction between interlayer excitons and correlated electrons in superlattice.
  -	Identified integer filling of Mott insulator and fractional fillings of Wigner crystals, with opposite valley polarization.
	
* *Metasurface Integrated 2D Material WSe2–SiN system for Photonic Crystal Cavities*                                
  - Fabricated SiN metasurface by LPCVD and inductive-coupled plasma etching. Coupled monolayer WSe2 to SiN metasurface.
  - Simulated the guided mode resonances (GMR) of the WSe2-SiN photonic crystal cavities by RCWA, FDTD and COMSOL. 
  - Performed Energy-Momentum Spectroscopy in self-built back-focal-plane imaging setup. Observed Rabi splitting of 18meV.
  - Demonstrated the existence of exciton–polariton with high Q factor~143, inspiring future applications in lasers and displays. 

* *Unit Valley Polarization Quantum Bits Control in WSe2/MoSe2 Heterostructure*                                       
  - Fabricated twisted heterostructure under microscope. Wrote electrodes by E-beam lithography. Characterized devices by AFM. 
  - Identified spin-triplet and singlet interlayer excitons with PL spectroscopy by tuning electric, magnetic field and temperature.
  - Conducted helicity resolved PLE spectroscopy, discovered 100% valley polarization for future quantum computing application

Research Projects in Machine Learning
--------------
* *Accelerating Decentralized Momentum SGD in Large-batch Deep Learning for Object Detection*
  - Conducted baseline model based on PmSGD and DmSGD for object detection on Cifar-10 and ImageNet dataset using Pytorch.
  - Derived convergence analysis of SGD models in both non-convex and strongly convex scenarios for algorithm optimization.
  - Evaluated performance of DecentLAM with state-of-art models (Faster-RCNN, YOLO) on COCO dataset, achieved linear speedup as PmSGD, reduced inconsistency bias exponentially by (1-β^2), saved 60% communication costs per iteration.

* *Stochastic Optimization and Data Compression in Distributed Learning for Image Classification*
  -	Developed deep learning model based on LeNet5 and FCNNs for image classification on Fashion-MNIST and Cifar10 datasets.
  -	Applied Top-k Sparsification and Low-bit Quantization for data compression, saved memory usage by 77%.
  -	Simulated the distributed/federated learning based on Error Compensated SGD, got 93.6% accuracy with 20% time reduction. 
     
Projects of Industry-related topics 
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

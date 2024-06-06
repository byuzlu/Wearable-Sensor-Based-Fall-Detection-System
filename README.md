# README

## Project Overview

This project involves analyzing wearable-sensor data to detect falls in real-time, minimizing related injuries and healthcare costs. The data, provided in "falldetection_dataset.csv," consists of 566 samples of motor actions (falls and non-falls) and 306 features reflecting properties like velocity, acceleration, temperature, and pressure. The analysis includes exploratory data analysis, clustering, and building classifiers to detect falls with high accuracy.

## Data Description

- **File:** falldetection_dataset.csv
- **Samples:** 566
- **Features:** 306 (velocity, acceleration, temperature, pressure)
- **Labels:** 'F' (fall) or 'NF' (non-fall)

## Exploratory Data Analysis

1. **Principal Components Analysis (PCA):**
   - Perform PCA on the 566x306 feature matrix.
   - Extract the top two principal components (PCs).
   - Note the variance captured by the top two PCs.

2. **Clustering:**
   - Using the projections of data samples onto the first and second PCs, run k-means clustering (or another method).
   - Experiment with different numbers of clusters (N).
   - Assess the proper number of clusters.
   - For N=2, check the percentage overlap/consistency between cluster memberships and the action labels.

## Supervised Learning

1. **Data Split:**
   - Implement a three-way split of data into non-overlapping training, validation, and testing sets (e.g., 70%, 15%, 15%).

2. **Model Training:**
   - **Support Vector Machine (SVM) Classifier:**
     - Experiment with various hyperparameters to maximize classification accuracy.
   - **Multi-Layer Perceptron (MLP) Classifier:**
     - Experiment with different hyperparameters to maximize classification accuracy.

3. **Cross-Validation:**
   - Fit models on the training set.
   - Perform parameter selection based on the validation set.
   - Report final classification accuracy on the testing set.

4. **Comparative Evaluation:**
   - Show/report all intermediate results.
   - Compare the performance of SVM and MLP models.
   - Comment on the success of fall detection based on wearable sensors.

## Conclusion

This project aims to provide insights into the effectiveness of wearable sensors for real-time fall detection. By performing PCA and clustering, followed by building and evaluating SVM and MLP classifiers, the goal is to achieve high accuracy in distinguishing falls from non-falls. The comparative analysis will help determine the best approach for reliable fall detection using wearable-sensor data.

## Contributions and Support

Contributions and feedback are welcome to enhance the functionality and accuracy of the fall detection models. For any questions or assistance, please reach out to baha.yuzlu@gmail.com. Thank you for your interest and support!

# Face-Recognition
This project implements a face recognition system using Principal Component Analysis (PCA) for dimensionality reduction and K-Nearest Neighbors (KNN) for classification.
The system processes facial images from the AT&T dataset (also known as the ORL dataset), performs feature extraction using PCA, and classifies faces using a KNN classifier with different neighbor configurations.

Features
Image Preprocessing: Reads and processes PGM image files from the dataset directory structure.
Dimensionality Reduction: Uses PCA to reduce the feature space while preserving variance (80% and 85% variance retention tested).
KNN Classification: Implements a KNN classifier with k values of 1, 3, 5, and 7 neighbors.
Performance Evaluation: Computes accuracy scores and provides detailed misclassification analysis.
Visualization: Plots accuracy trends across different k-values for comparison.

Dataset
The project uses the AT&T face dataset, which contains 400 images of 40 distinct subjects (10 images per subject). Images are stored in PGM format with a resolution of 112x92 pixels (10304 features per image).

Requirements
Python 3.x
NumPy
Matplotlib
scikit-learn
Pillow (PIL)
OS module (built-in)

Usage
Place the dataset in the appropriate directory (update the path in Read_pgm function if necessary).
Run the notebook to preprocess images, perform PCA, and evaluate the KNN classifier.
Results include accuracy scores for each k-value and a plot showing accuracy trends.

Results
The system achieves high accuracy (up to 94.5% with k=1 and 80% variance retention), with detailed output showing classifications and misclassifications for each test instance.

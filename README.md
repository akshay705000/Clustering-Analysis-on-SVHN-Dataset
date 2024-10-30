
# Clustering Analysis on SVHN Dataset

This project performs clustering analysis on the Street View House Numbers (SVHN) dataset, utilizing both PCA and clustering algorithms to analyze and visualize digit images. The project compares clustering quality on raw and PCA-reduced data using k-NN and K-Means, providing insights into dimensionality reduction and clustering effectiveness.

## Table of Contents
- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Installation](#installation)
- [Usage](#usage)
- [Data Description](#data-description)
- [Results](#results)

## Introduction
This clustering assignment applies **k-NN** and **K-Means** clustering to the **SVHN dataset**, a dataset of digit images in street scenes. The analysis focuses on the effectiveness of clustering before and after applying PCA for dimensionality reduction, with comparisons on cluster quality and classification accuracy.

## Project Overview
- **Dimensionality Reduction**: Applied **Principal Component Analysis (PCA)** on the SVHN dataset to visualize the percentage of variance (PoV) explained and reduce the dataset's dimensionality.
- **Clustering and Evaluation**:
  - **k-Nearest Neighbors (k-NN)**: Evaluated k-NN accuracy on both raw data and PCA-reduced data to observe classification performance changes.
  - **K-Means Clustering**: Implemented K-Means clustering on both raw and PCA-reduced datasets, assessing clustering quality and comparing results to k-NN accuracy.

## Installation
To get started, make sure you have the required libraries. All necessary imports are included in the provided notebook, but if using another IDE, install the libraries as follows:
```bash
pip install scikit-learn pandas numpy
```

## Usage
1. **Open Google Colab**: Visit [Google Colab](https://colab.research.google.com/).
2. **Upload Data Files**:
   - Click on the "Open Colab" button.
   - Click "Upload" and then "Browse" to select `train_32x32.mat` and `test_32x32.mat` files.
   - Upload these files to **session storage** (do not upload to any other folder).
3. **Run the Notebook**:
   - Run all cells in sequence as directed in the notebook.

## Data Description
- **SVHN Dataset**: Contains digit images from street views, organized into 10 classes (one for each digit from 0 to 9). Digit labels range from `0` to `9`, with:
  - **Training Set**: 73,257 images.
  - **Test Set**: 26,032 images.

- **Training Subset**: This analysis uses a subset of the original training data, consisting of 2,500 randomly selected samples per class (totaling 25,000 samples). The test set remains unchanged with 26,032 samples.

## Results
- **PCA Analysis**: Visualized the Percentage of Variance (PoV) explained by each component and selected optimal dimensions for clustering.
- **Clustering Performance**:
  - Compared k-NN accuracy and clustering quality between raw and PCA-reduced datasets.
  - Observed and evaluated clustering effectiveness using metrics such as inertia and silhouette scores.

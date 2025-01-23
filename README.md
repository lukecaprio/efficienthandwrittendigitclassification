# Handwritten Digit Classification: K-Means and K-Nearest Neighbors (KNN)

This project explores handwritten digit classification using a combination of **K-Means Clustering** and **K-Nearest Neighbors (KNN)**. The goal is to enhance classification performance by clustering digits into groups and using the cluster centers to train a simplified KNN model. The implementation includes visualizations of clustering results, performance analysis, and comparisons with a baseline KNN model trained on the full dataset.

## Project Structure

The repository is organized as follows:

- **`Digit_Recognition_Using_Machine_Learning_Algorithms_K_Means_Clustering_and_K_Nearest_Neighbors.ipynb`**  
  - Jupyter Notebook containing the complete implementation of the project. This includes:
    - Loading and preprocessing the MNIST dataset.
    - Clustering digit images using K-Means and visualizing cluster centers.
    - Training and evaluating a KNN model using cluster centers as training data.
    - Comparing the performance of the KNN model with and without K-Means preprocessing.
    - Visualizing results using confusion matrices and accuracy metrics.

- **`data/`** *(Optional: Include this if dataset-related files are provided)*  
  - Directory for any pre-downloaded or processed data files used in the project.

- **`requirements.txt`**  
  - List of dependencies for setting up the project environment.

## Features

- **K-Means Clustering**: Groups digit images into clusters to capture intra-digit variations and generate cluster centers as training data.
- **K-Nearest Neighbors (KNN)**: Classifies handwritten digits using the clustered data and compares its performance to a generic KNN model.
- **Data Preprocessing**: Includes normalization, reshaping, and grouping of images based on their labels.
- **Visualization**:
  - Visualizes digit frequencies in the dataset.
  - Displays K-Means cluster centers to analyze digit patterns.
  - Generates confusion matrices to evaluate model performance.

## Results

- **Baseline KNN Model**:
  - Achieved accuracy: ~97%
  - Trained on the full MNIST dataset without clustering.

- **K-Means + KNN Model**:
  - Reduced training data to cluster centers.
  - Achieved comparable accuracy (~98%) with significantly improved prediction speed.

## Prerequisites

- Python 3.8 or higher
- Required libraries: `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `tensorflow`

Install dependencies using:
```bash
pip install -r requirements.txt

# Spotify Song Likability Prediction Project

## Introduction
This project focuses on predicting whether a Spotify user will like or dislike a song using a dataset containing various song features. The goal is to explore the dataset, preprocess it, and develop a predictive model using **Logistic Regression** to determine song likability based on features like liveliness, acoustics, and energy.

All algorithms, including **Logistic Regression** and **K-Means Clustering**, have been implemented from scratch without using any pre-built machine learning libraries, ensuring a deep understanding of their workings.

We will perform the following steps:
- Data acquisition and preprocessing
- Exploratory Data Analysis (EDA)
- K-Means clustering for song grouping
- Logistic Regression implementation for prediction
- Analysis of the model’s performance

The project is implemented using **pandas**, **NumPy**, and **matplotlib** for data handling, preprocessing, and visualization. Through this process, we aim to reveal key factors influencing song likability for Spotify users.

## Methodology

### 1. Dataset Acquisition
- The dataset consists of a Spotify user’s liked and disliked songs, stored in a CSV file.
- Features include attributes such as:
  - Liveliness
  - Acoustics
  - Energy
  - Danceability
  - Loudness
  - Speechiness
  - Duration

### 2. Data Preprocessing
- **Handling Missing Values**: Missing values are handled either by removing incomplete records or imputing missing data with appropriate strategies.
- **Feature Scaling**: Normalize features to ensure consistent scaling and prevent any feature from disproportionately influencing the model.

### 3. Data Preparation
- **Data Split**: The dataset is split into training and testing sets to properly evaluate the model’s performance.
- **Feature Scaling**: Feature scaling is performed to standardize the range of input features, improving model performance.

### 4. Exploratory Data Analysis (EDA)
- **Histograms & Count Plots**: Visualize the distribution of song features using histograms and count plots to understand their behavior.
- **Correlation Matrix**: Generate a correlation matrix to identify relationships between features and their impact on song likability.

### 5. K-Means Clustering
- Apply **K-Means Clustering** to group songs into clusters based on feature similarities.
- Identify which cluster contains the highest number of liked songs, revealing common patterns.
- The **K-Means Clustering** algorithm has been implemented from scratch to demonstrate how clustering works step-by-step.

### 6. Logistic Regression Implementation
- Create a custom class for **Logistic Regression**, implemented entirely from scratch, including:
  - **Sigmoid Function**: To calculate the probability of a song being liked.
  - **Fit Function**: For model training and optimizing the coefficients using gradient descent.
  - **Predict Function**: To predict whether a user likes or dislikes a song.
  
### 7. Analysis of Logistic Regression Results
- **Confusion Matrix**: Evaluate model performance using a confusion matrix, which shows how well the model predicts song likability.
- **Accuracy Calculation**: Define a function to calculate the model’s accuracy and overall performance.

## Results

### Conclusion
In this project, we explored a Spotify user’s song preferences, performing data analysis and model development to predict likability. Key insights include:
- **Correlation Analysis**: The user tends to prefer songs with higher danceability, loudness, and speechiness while avoiding longer compositions and instrument-heavy tracks.
- **K-Means Clustering**: Three distinct music clusters were identified, each representing a unique musical style, with one cluster containing the majority of liked songs.
- **Logistic Regression Model**: The model achieved an accuracy of **84.6%** in classifying liked songs. This suggests a strong ability to predict song likability based on the provided features.

### Implications
These findings not only help us understand the user’s musical preferences but also provide valuable insights for refining recommendation systems and personalizing the user experience on Spotify.

### Dataset
The dataset has been taken from [Kaggle](https://www.kaggle.com/datasets/bricevergnou/spotify-recommendation)

# Stock Sentiment Analysis and Price Prediction

This project explores the potential of sentiment analysis in predicting stock prices, specifically focusing on Microsoft Corporation (Microsoft). By leveraging the BERT (Bidirectional Encoder Representations from Transformers) model, we analyze sentiment in news articles related to Microsoft and incorporate it into a neural network for daily stock price prediction.

## Introduction

Sentiment analysis has gained attention in stock-related news, but its application to stock price prediction is limited. This study introduces a scoring technique that combines sentiment analysis results with the influence of news from previous days. We utilize the New York Times API to collect Microsoft-related news articles and incorporate macroeconomic indicators into our prediction model.

## Methodology

1. Data Collection:
   - Utilize the New York Times API to scrape Microsoft-related news articles.
   - Gather historical Microsoft stock prices from Yahoo Finance.

2. Sentiment Analysis:
   - Use BERT to analyze sentiment in the news articles.
   - Fine-tune BERT using a financial news dataset for sentiment labeling.

3. Scoring Technique:
   - Develop a scoring function that considers sentiment analysis results and the influence of previous days' news.
   - Apply various aggregation methods to capture the lasting impact of news.

4. Neural Network Model:
   - Incorporate sentiment scores and other stock-related features into a neural network.
   - Utilize LSTM for time-series modeling of stock prices.

## Results and Challenges

Our approach reduces the RMSE of stock price prediction by 7% compared to the baseline model. However, challenges include limited labeled data for Microsoft-related news articles and resource-intensive evaluation processes. Despite these challenges, this research demonstrates the potential of sentiment analysis in stock price prediction and motivates further exploration in this field.

## Repository Structure

- `data/`: Directory for storing collected data.
- `models/`: Directory containing pre-trained models.
- `notebooks/`: Jupyter notebooks documenting experiments.
- `scripts/`: Scripts for data preprocessing and model training.
- `results/`: Directory to store analysis results.
- `README.md`: Detailed project overview and instructions.

For detailed implementation and experimental results, refer to the notebooks and code in the repository.

[GitLab Repository Link](https://git.uwaterloo.ca/ky5liu/cs679_project)

Note: The repository includes code and progress made during experiments, providing insights for future research.

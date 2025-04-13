# Stock Price Prediction with Financial News Sentiment Analysis

A data science project exploring how financial news sentiment can enhance traditional stock price prediction models, focusing on Microsoft stock movements.

## Project Overview

This project implements a complete machine learning pipeline that:
- Combines market data with financial news headlines
- Compares traditional ML models with deep learning approaches
- Evaluates the impact of sentiment analysis on prediction accuracy
- Demonstrates advanced time-series analysis techniques

## Key Findings

| Model | Without Sentiment | With Sentiment |
|-------|-------------------|----------------|
| Logistic Regression | 86.27% | 84.31% |
| Random Forest | 52.94% | 50.98% |
| LSTM | 95.28% | 95.38% |

**Insights:**
- LSTM networks demonstrated superior performance for price prediction
- Logistic Regression performed surprisingly well for trend classification
- News sentiment had minimal impact on prediction accuracy
- Time-series analysis proved most effective for forecasting

## Technologies

- Python (3.8-3.11)
- pandas, numpy for data manipulation
- scikit-learn for traditional ML models
- TensorFlow for LSTM implementation
- NLTK for sentiment analysis
- yfinance for market data
- Matplotlib, Seaborn for visualization

## Project Structure

```
stock-prediction-project/
├── data/                      # News headlines datasets
├── Notebooks/                 # Analysis code
│   └── Final_Project.ipynb    # Main notebook
├── README.md                  # Documentation
└── requirements.txt           # Dependencies
```

## Setup and Usage

### Requirements
- Python 3.8-3.11 (TensorFlow compatibility requirement)

### Installation

```bash
# Clone repository
git clone https://github.com/benbelaish/stock_prediction_project.git
cd stock_prediction_project

# Install dependencies
pip install -r requirements.txt

# Run the analysis
python -m jupyterlab
```

After launching JupyterLab, navigate to the Notebooks directory and open Final_Project.ipynb.

## Implementation Details

The analysis follows these key steps:
1. Data acquisition (stock prices and news headlines)
2. Text preprocessing and sentiment extraction
3. Feature engineering and model preparation
4. Model training and evaluation
5. Comparative analysis of results

## About the Author

Ben Belaish - Data Analyst specializing in financial markets and predictive modeling.

Contact: benbelaish123@gmail.com

---

*This project is for educational purposes only and should not be used for investment decisions.*

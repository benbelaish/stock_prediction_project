# Stock Price Prediction with News Sentiment Analysis

A data science project examining how financial news sentiment impacts stock price prediction models for Microsoft.

## 📊 Overview

This project combines stock market data with financial news sentiment to predict price movements using:
- Traditional ML models (Logistic Regression, Random Forest)
- Deep learning (LSTM neural networks)
- News headline sentiment analysis

## 🔍 Key Findings

| Model | Without Sentiment | With Sentiment |
|-------|-------------------|----------------|
| Logistic Regression | 86.27% | 84.31% |
| Random Forest | 52.94% | 50.98% |
| LSTM | 95.28% | 95.38% |

- LSTM significantly outperformed traditional methods for price prediction
- News sentiment had minimal impact on prediction accuracy
- Time-series features were the strongest predictors of price movements

## 📋 Methodology

The project follows a systematic approach to analyze financial data and sentiment:

### 1. Data Acquisition & Preprocessing
- **Market Data**: Daily OHLCV data from yfinance
- **News Data**: Headlines from CNBC, Guardian, and Reuters
- **Preprocessing**: Datetime standardization and feature engineering 

### 2. Traditional ML Approach
- Feature selection (Open, Close, Low, High, Volume)
- Train/test split (80/20) preserving time order
- StandardScaler normalization
- Logistic Regression and Random Forest models for trend prediction

### 3. LSTM Implementation
- 5-day window sequence creation
- Two-layer LSTM with dropout for regularization
- Adam optimizer with early stopping
- MAPE (Mean Absolute Percentage Error) for evaluation

### 4. Sentiment Analysis
- Text preprocessing with NLTK (tokenization, lemmatization, stopwords)
- Unsupervised sentiment scoring using a pre-trained LSTM
- Daily sentiment aggregation and feature integration

### 5. Comparative Evaluation
- Cross-model performance comparison with and without sentiment
- Overfitting assessment using train vs. test accuracy
- Final analysis of sentiment contribution to prediction accuracy

## 🛠️ Technologies

- Python 3.8-3.11
- pandas, numpy, matplotlib, seaborn
- scikit-learn, TensorFlow
- NLTK for text processing
- yfinance for market data

## 📂 Project Structure

```
stock-prediction-project/
├── Data/                      # News headlines datasets
├── Notebooks/                 # Analysis code
│   └── stocks_final_project.py
├── README.md
└── requirements.txt           # Dependencies
```

## 🚀 Setup and Usage

```bash
# Clone repository
git clone https://github.com/benbelaish/stock_prediction_project.git

# Install dependencies
pip install -r requirements.txt

# Run the analysis with JupyterLab
python -m jupyterlab
```

Navigate to the Notebooks directory and open the main analysis file.

## ⚠️ Methodological Note

Results may vary slightly between different environments (local Jupyter vs. Google Colab) due to probabilistic algorithms and library versions, but conclusions remain consistent.

## 👨‍💻 About the Author

Ben Belaish - Data Analyst specializing in financial markets and predictive modeling.

Contact: benbelaish123@gmail.com

---

*This project is for educational purposes only.*

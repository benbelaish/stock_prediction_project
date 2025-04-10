<div dir="ltr">

# Stock Price Prediction with News Sentiment Analysis

A data science project predicting Microsoft stock movements using machine learning models enhanced with financial news sentiment analysis.

## 📊 Overview

This project combines stock market data with financial news headlines to predict price movements using:
- Traditional ML models (Logistic Regression, Random Forest)
- Deep learning (LSTM neural networks)
- News headline sentiment analysisש

## 🔍 Key Findings

| Model | Without Sentiment | With Sentiment |
|-------|-------------------|----------------|
| Logistic Regression | 86.27% | 84.31% |
| Random Forest | 52.94% | 50.98% |
| LSTM | 95.28% | 95.38% |

- LSTM models significantly outperformed traditional methods for precise price prediction
- Logistic Regression performed surprisingly well for trend classification
- News sentiment had minimal impact on prediction accuracy (slightly decreased performance for Logistic Regression and Random Forest)
- Time-series analysis proved most effective for price forecasting

## 🛠️ Technologies

- Python, pandas, numpy
- scikit-learn, TensorFlow
- NLTK for headline processing
- yfinance for market data
- Matplotlib, Seaborn for visualization

## 📂 Project Structure

```
stock-prediction-project/
├── data/                      # News headlines datasets
│   ├── cnbc_headlines.csv     # CNBC news headlines
│   ├── guardian_headlines.csv # Guardian news headlines
│   └── reuters_headlines.csv  # Reuters news headlines
├── notebooks/                 # Analysis code
│   └── stocks_final_project.py
├── README.md                  # Project documentation
└── requirements.txt           # Dependencies
```

## 🚀 Setup

```bash
# Clone repository
git clone https://github.com/benbelaish/stock-prediction-project.git

# Install dependencies
pip install -r requirements.txt

# Run analysis
python notebooks/stocks_final_project.py
```

## 📈 Key Insights

Based on model performance:

- **LSTM Superior for Price Forecasting**: With ~95% accuracy, the LSTM model shows excellent capability for precise price prediction.
- **Effective Feature Set**: Using Open, Close, High, Low, and Volume as features provides good predictive power.
- **Classical vs Deep Learning**: While LSTM excels at exact value prediction, Logistic Regression is effective for trend direction.
- **Sentiment Analysis Limitations**: The sentiment analysis approach used didn't significantly improve prediction accuracy, suggesting either that:
  - News sentiment isn't a strong predictor for this specific stock
  - Our sentiment extraction method needs refinement
  - The time window for sentiment impact may need adjustment

As concluded in the analysis:
> "LSTM model is good at predicting exact values, while classical models are good at predicting trends. Using multiple models together can give a more complete picture."

## 👨‍💻 About Me

Project by Ben Belaish, a data analyst with focus on financial markets and predictive modeling.

**Contact**: [benbelaish123@gmail.com]

---

*This project is for educational purposes only and should not be used for investment decisions.*


<div dir="ltr">

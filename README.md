# Macro-Economic Pulse: Inflation & Real Interest Rate Analyzer

## 1. Problem & User

This project builds an interactive Streamlit tool to analyze and forecast the relationship between annual inflation and real interest rates. It is designed for economics students, junior financial analysts, and users who want a simple and interactive way to understand how central bank policies react to price changes across major global economies over time.

## 2. Data

- **Source:** Macroeconomic indicators based on World Bank Open Data parameters
- **Access date:** 23 April 2024
- **Subject:** Macroeconomics
- **Final sample countries:** China, Germany, Japan, United Kingdom, and United States
- **Time period:** 2010–2023

The project utilizes annual macroeconomic time-series data and retains the key variables required for policy sensitivity analysis, including:

- Year
- Country
- Inflation Rate (%)
- Real Interest Rate (%)
- Inflation Volatility (calculated via rolling standard deviation)

## 3. Methods

This project uses Python to:

1. create a robust structured dataset for macroeconomic analysis
2. clean and prepare the time-series dataset using Pandas
3. calculate policy sensitivity using Machine Learning (Linear Regression)
4. generate OLS trendlines and dynamic visual comparisons
5. build an interactive Streamlit tool for user exploration and stress testing

The key indicators used are:

- Annual Inflation (%)
- Real Interest Rate (%)
- Policy Sensitivity Score (ML-based)
- Historical Volatility (σ)

These metrics are used to compare three dimensions of economic performance:

- price stability
- monetary policy responsiveness
- real financial returns

## 4. Key Findings

- **Inverse Correlation:** A strong negative relationship exists between inflation and real interest rates across most selected economies.
- **Policy Lag:** Real interest rates frequently turn negative when nominal rate adjustments fail to offset rapid inflation.
- **Regional Divergence:** Japan exhibits a unique low-inflation stability profile compared to the high volatility observed in Western markets.
- **Predictive Insight:** The ML model suggests significant erosion of real returns once the inflation threshold exceeds 4%.

## 5. How to Run

1. Install required libraries: `pip install -r requirements.txt`
2. Run the application: `streamlit run app.py`

## 6. Project Links

- **Live Tool:** [(https://acc102-macro-analysis-ruqma5q2bpwvk2exwxesjp.streamlit.app/)]
- **GitHub Repository:** [(https://github.com/ZDJ020314/ACC102-Macro-Analysis)]
- **Demo Video:** [(https://www.bilibili.com/video/BV17rorBREnX/?spm_id_from=333.1387.homepage.video_card.click&vd_source=82929e68059eea32b530ffb601bc64fe)]

## 7. Limitations & Next Steps

- **Limitations:** The current predictive module uses linear regression which may not capture non-linear "Black Swan" events.
- **Next Steps:** Future versions will integrate GDP growth data and implement ARIMA models for improved time-series forecasting.

# PJM-Energy-Forecast-GenAi
PJM energy forecasting dashboard using XGBoost and GenAI. Accurate 30-day load forecasts, scenario analysis, interactive Q&amp;A, and business report generation for PJM grid data.

🚀 Overview
This project delivers a robust, business-ready dashboard for forecasting hourly energy demand across the PJM Interconnection (covering 13 US states and DC), using advanced machine learning and GenAI:

XGBoost-based 30-day hourly load forecasting (MAPE ≈ 1%).

Scenario analysis: Simulate uncertainty and demand shifts.

Peak detection, trend insights, and downloadable reports.

GenAI (Llama-3) integration: Ask natural language questions about forecasts or the full dataset, and get automated business reports.

🗂️ Dataset
PJMW_hourly.csv (sample) and PJMW_MW_Hourly.xlsx (sample)

Columns: Datetime, MW (hourly grid load, MW)

Coverage: 2002–2011, hourly data for the full PJM grid.

✨ Features
Forecasting tab:

Generate 30-day hourly load forecasts with XGBoost.

Adjust uncertainty (MAPE %) and simulate demand shifts.

Visualize confidence intervals, peaks, and trends.

Download CSV and TXT business reports.

GenAI chatbot: Ask business questions about the forecast.

Dataset analytics tab:

Explore and visualize the full PJM dataset.

GenAI Q&A: Ask any question about historical patterns, peaks, trends, and more.

Download GenAI-generated business reports.

⚡ Quick Start
Clone this repo:

bash
git clone [https://github.com/yourusername/pjm-energy-forecast-genai.git
cd pjm-energy-forecast-genai](https://github.com/Jeetibp/PJM-Energy-Forecast-GenAi/blob/main/README.md)
Add your data:

Place PJMW_hourly.csv or PJMW_MW_Hourly.xlsx in the project root.

Set up Hugging Face API key:

Create .streamlit/secrets.toml and add:

text
[hf_token]
hf_token = "YOUR_HUGGINGFACE_TOKEN"
Install requirements:

bash
pip install -r requirements.txt
Run the app:

bash
streamlit run app.py
💡 Example GenAI Questions
What is the highest demand day in the forecast?

What is the average demand for July?

Are there any seasonal trends or unusual patterns?

How does demand change on weekends vs weekdays?

Generate a summary report for the last year.

🛠️ Tech Stack
Python, Streamlit, XGBoost

Hugging Face Inference API (Llama-3)

Pandas, Plotly, joblib

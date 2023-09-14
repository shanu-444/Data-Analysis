# Data-Analysis
This is my first repository and it consists some data analysis projects
Author - Pratik Shukla

import yfinance as yf
import pandas as pd
import plotly.graph_objects as go

# TESLA STOCKS

tick = 'TSLA'
tsla = yf.download(tick)
tsla.head()

# GME STOCKS

gme_data = yf.download(tick)

import plotly.graph_objects as go

from datetime import datetime

df = pd.read_csv('https://raw.githubusercontent.com/plotly/datasets/master/finance-charts-apple.csv')

fig = go.Figure(data=[go.Candlestick(x=df['Date'],
                open=df['AAPL.Open'],
                high=df['AAPL.High'],
                low=df['AAPL.Low'],
                close=df['AAPL.Close'])])

fig.show()

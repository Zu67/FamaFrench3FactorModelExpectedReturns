# Fama French 3 factor Expected Returns on US equity security

One notebook, `Fama French 3 factor Expected Returns on US equity security.ipynb`, committed on 2021-07-12 by Zu67 with the message "Add files via upload". The notebook has no saved output.

The code cell requests monthly adjusted closes for Macy's (ticker M) from Yahoo Finance starting 2016-07-01, takes the last 60 months of monthly Fama-French 3-factor data via getFamaFrenchFactors, merges the two tables on year and month, fits an OLS of excess return on Mkt-RF, and draws a scatter plot.

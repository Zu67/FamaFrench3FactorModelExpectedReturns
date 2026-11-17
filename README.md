# Fama French 3 factor Expected Returns on US equity security

One notebook, `notebook/Fama French 3 factor Expected Returns on US equity security.ipynb`. Zu67 uploaded it at the repository root on 2021-07-12 with the message "Add files via upload". The notebook has no saved output.

The cell imports pandas, numpy, matplotlib, and datetime, then has a bare `pip install getFamaFrenchFactors` line. It calls `DataReader`, `end`, `macydata`, `macydataF`, and `gff`, and none of those names are assigned in the cell, so it does not run as written.

The lines that are there request monthly adjusted closes for Macy's (ticker M) from Yahoo Finance starting 2016-07-01, take the last 60 months of monthly Fama-French factors, and merge the tables on year and month. After sorting newest first, `rM` is this row's adjusted close divided by the next row's close, minus 1. `rMkt` is `Mkt-RF` plus `RF`. The scatter plots `rMkt` against the adjusted close, not against `rM`. The red line is a straight fit of `rM` on `rMkt`. Separately, the OLS regresses `rM` minus `RF` on `Mkt-RF` with a constant.

- ` Hidden Markov Model (HMM).ipynb `:**    

This notebook wraps the entire experimental pipeline in a single script so that the thesis can be reproduced top‑to‑bottom with one run.  Key contents:

Data Load & Validation — reads combined_data.xlsx, re‑indexes to custom NYSE trading calendar, and sanity‑checks each series.

Reusable Utility Functions

kim_smoother, forward_filter_tmstgarch_pq – hidden‑state smoothing & likelihood evaluation

make_strategy_df, ann_return, sharpe_ratio, max_drawdown – performance metrics

High‑level helper build_strat() that returns a tidy DataFrame suitable for LaTeX export.

Daily / Monthly Experiments — loops through the same eight candidate factors, automatically:

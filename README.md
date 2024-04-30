## Steps to Follow 

# Packages Needed:
    import yfinance as yf
    import pandas as pd
    import numpy as np
    import matplotlib.pyplot as plt
    import plotly.express as px

# Review Parts in this Order
    1. Finish Reading the README.md
    2. Read the FINAL PROPOSAL
    3. Read the Overview
    4. Load the Builder.ipynb
    5. Read the Concluding Analysis 

# Key information:
    - Analysis is based off year 2020 - 2023
    - Wilshire 5000 used as an index
    - S&P Returns used as an index
    - Risk free assumption in Efficient Frontier analysis is 4%
    - Code lines 2, 3, 8, 9, 10 will take over an hour to run together

# CSV files breakdown
    - Wilkshire_5000.csv : Lists firms in the Wilshire 5000 
    - net_income_data_grouped.csv : Lists firms and 4 years of Net Income 
    - dividend_data_grouped.csv: Lists firms and 4 years of Dividend Information
    - merged_data.csv: Merged "net_income_data_grouped.csv" + "dividend_data_grouped.csv" based on Ticker
    - Slow_Grow_Master.csv : Renamed "merged_data.csv" with an updated 1st column of name of Ticker
    - modified_net_income_data.csv: Adds Net Income Growth Columns to "net_income_data_grouped.csv"
    - ticker_2023_PE.csv: Creates a list of Ticker PE ratios
    - ticker_Gsector.csv: Creates a list of Ticker Gsectors
    - ticker_2023_MarketCap.csv: Creates a list of Ticker Market Capitalizations
    - PE_Gsector.csv: Merges the "ticker_Gsector.csv" + "ticker_2023_PE.csv" on the Ticker column
    - PE_Gsector_with_avg.csv: Adds the avgerage PE grouped by Gsector column to "PE_Gsector.csv"
    - cleaned_PE_Gsector_with_avg.csv: Cleans the "PE_Gsector_with_avg.csv" removing items messing with the calculation
    - ticker_2023_MarketCap_with_Category.csv: Adds a categorization to "ticker_2023_MarketCap.csv"
    - Stalwart_Master.csv: Combines "ticker_2023_MarketCap_with_Category.csv" + "cleaned_PE_Gsector_with_avg.csv" + "modified_net_income_data.csv" on the Ticker column
    - NI_Grow_PE.csv: combines the "modified_net_income_data.csv" + "ticker_2023_PE.csv" on Ticker
    - Fast_Grower_Master.csv: Adds an optimal growth column to "NI_Grow_PE.csv"
    - Clean_Slow_Grow_Master.csv: cleans "Slow_Grow_Master.csv" by dropping missing values 
    - Clean_Fast_Grower_Master.csv: cleans "Fast_Grower_Master.csv" by dropping missing values 
    - Clean_Stalwart_Master.csv: cleans "Stalwart_Master.csv" by dropping missing values 
    - Screened_Slow_Grow.csv: Screens the "Clean_Slow_Grow_Master.csv" based on Lynch's Criteria
    - Screened_Stalwart.csv: Screens the "Clean_Stalwart_Master.csv" based on Lynch's Criteria
    - Screened_Fast_Grower.csv: Screens the "Clean_Fast_Grower_Master.csv" based on Lynch's Criteria

    





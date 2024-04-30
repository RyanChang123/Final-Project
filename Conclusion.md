### Concluding Thoughts

## Peter Lynch Overview:

    Peter Lynch is a legendary investor known for his exceptional success managing the Fidelity Magellan Fund from 1977 to
    1990. Born on January 19, 1944, Lynch graduated from Boston College in 1965 with a degree in finance and later earned a
    Master of Business Administration (MBA) from the Wharton School at the University of Pennsylvania.
    
    Lynch joined Fidelity Investments in 1969 as an intern and eventually became the head of the Magellan Fund in 1977. Under
    his management, the fund grew from $18 million in assets to over $14 billion, making it one of the largest and most
    successful mutual funds in the world at the time.
    
    During his tenure at Magellan, Lynch achieved an average annual return of around 29%. His success made him one of the most
    respected and influential investors of his time. After retiring from Fidelity in 1990, Lynch continued to be active in the
    investment community through writing books and giving talks on investing strategies. His book One Up on Wall Street was the
    inspiriation for this project.

## Peter Lynch's 6 Invesment Groups 

    1. Slow Growers: Companies paying dividens 
    2. Stalwarts: Stable Companies who are established in the industry
    3. Fast Growers: Companies in a rapid growth stage
    4. Cyclical: Companies heavily influenced by seasonality
    5. Turnarounds: Distressed companies
    6. Asset Plays: Companies with an asset sheet largely of fixed assets
        
    The focus of this project was on the first three given their quantitative nature.
    
## Conclusion 
    
    In the analysis section of the Builder.ipynb the normalized index chart outlined the returns of the screened companies 
    compared to the returns on the indexes. The results are astounding as all screened categories outperformed the S&P 
    and  wilshire 5000 over the same time span.
         - Results 
            1. Slow Grower        |CAGR: 12.98%
            2. Stalwart           |CAGR: 19.42%
            3. Fast Grower        |CAGR: 13.08%
            4. S&P 500            |CAGR: 8.29% 
            5. Wilshire 5000      |CAGR: 6.97%
        
## Efficient frontier analysis

  # Slow Grower
      - The optimal portfolio for Slow Grower had a very large concentration in AMAT and AMKR. More intersting, contrary to   what one would think, the volatility of the group seemed to be the largest out of any efficicent market analysis. This is suprising given the idea that dividens stabalize stock prices. Addtionally, the large returns in the tail of the simulated portfolios were more dramatic than the other categories. 
      - Results 
            Number of simulations: 20000
                Best Sharpe Ratio Portfolio:
                Return: 0.3042
                Volatility: 0.3908
                Sharpe Ratio: 0.676
                Weightage Breakdown:
                    ALSN: 2.05 %
                    ALX: 1.4 %
                    AMAL: 7.12 %
                    AMAT: 39.55 %
                    AMGN: 6.58 %
                    AMH: 9.59 %
                    AMKR: 33.7 %
                    
  # Stalwart
      - The optimal portfolio for Stalwart had the largest concetration in COST and ODFL. Moreover, the category had the highest simulated sharpe ratio out of any of the groups. This indicates that the Stalwart provides the best return for risk taken out of any of the groups. 
      - Results 
            Number of simulations: 20000
                Best Sharpe Ratio Portfolio:
                Return: 0.2829
                Volatility: 0.2593
                Sharpe Ratio: 0.9371
                Weightage Breakdown:
                    CCI: 1.0 %
                    COST: 45.36 %
                    ODFL: 43.75 %
                    TDG: 4.72 %
                    WAB: 5.17 %
                    
  # Fast Grower
      - The optimal portfolio for Fast Grower had the most variety of concentration among securities. More intersting, contrary to what one would think, the volatility of the group seemed to be the lowest out of any efficicent market analysis. This is suprising given the idea that smaller faster growing companies often have stock swings. Addtionally, fast growing companies are often expected to five excess returns based on the elevateed risk. However, this does not seem to be the case for this analysis. 
      - Results 
            Number of simulations: 20000
                Best Sharpe Ratio Portfolio:
                Return: 0.2368
                Volatility: 0.2569
                Sharpe Ratio: 0.7663
                Weightage Breakdown:
                    A: 0.19 %
                    AAPL: 40.66 %
                    BRO: 19.88 %
                    CRAI: 11.7 %
                    CW: 1.75 %
                    KEYS: 0.84 %
                    LSTR: 1.44 %
                    MSI: 14.16 %
                    ROG: 1.1 %
                    RPM: 8.29 %
    
# Future Improvement

    In the future I hope to find a way to screen the other methodologies used by Peter Lynch. Addtionally, focusing on
    international companies along with US companies would provide a more hollistic overview on the capabilities of his
    screening criteria. Futhermore, additional backtesting of would be important to truly understand returns. There was a 
    the amount of information that could be gathered from yfinance CRSP could be better in the future. Additonally, utilizing
    the screening methodology on future looking dates could also provide more insights into how returns are impacted by the
    screening criterion. 
    
    
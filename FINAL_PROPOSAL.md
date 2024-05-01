# RESEARCH PROPOSAL: Performance of Wilshire 5000 Firms Screened Through Peter Lynch's Methodology vs. Broader Market

## By Ryan Chang

## Peter Lynch Overview:

Peter Lynch is a legendary investor known for his exceptional success managing the Fidelity Magellan Fund from 1977 to 1990. Born on January 19, 1944, Lynch graduated from Boston College in 1965 with a degree in finance and later earned a Master of Business Administration (MBA) from the Wharton School at the University of Pennsylvania.

Lynch joined Fidelity Investments in 1969 as an intern and eventually became the head of the Magellan Fund in 1977. Under his management, the fund grew from $18 million in assets to over $14 billion, making it one of the largest and most successful mutual funds in the world at the time.

During his tenure at Magellan, Lynch achieved an average annual return of around 29%. His success made him one of the most respected and influential investors of his time. After retiring from Fidelity in 1990, Lynch continued to be active in the investment community through writing books and giving talks on investing strategies. His book "One Up on Wall Street" was the inspiration for this project.

### Research Question

In this research I am exploring how do firms screened through Peter Lynch's Slow Grower, Stalwart, and Faster Grower methodology compare to the broader market. My hypothesis is that the screened companies will have historically outperform the Wilshire 5000.

#### Report File

To accomplish this, The Report File will Consist of 4 Sections:

1. **Methodology Outline**
   - Peter Lynch background
   - Slow Grower, Stalwort, Fast Grower methodology breakdown
2. **Data Collection**
   - Data collection from Yahoo Finance
   - Data transformation steps
3. **Data Screening**
   - Finalization of screening 
   - Information regarding screening findings
4. **Final Analysis** 
   - Comparison to Wilshire return
   - Breakdown of comparison by screening criterion
   - Final conclusion and analysis
 
### Necessary Data

- **One Up On Wall Street**: Peter Lynch's book.
  - **Source:** [One Up on Wall Street](https://yourknowledgedigest.files.wordpress.com/2020/04/one-up-on-wall-street.pdf)
- **Wilshire 5000 Stock List**: Wilshire 5000 stock list.
  - **Source:**  [Wilshire 5000 List](https://info.wilshire.com/Wilshire-5000-Index-Fund-Holdings)
- **Stock Data**: Key Stock Information.
  - **Source:** Yahoo Finance
- **Wilshire 5000**: Performance from 2020-2023.
  - **Source:** Yahoo Finance

### Final Datasets

**Slow Growers**: 

- Key Information:
  - Year End Data for 5 years (2020-2023)
  - Were Dividends Paid?
  - Dividends Growth Year over Year
  
| Ticker | 2020_NI | 2021_NI | 2022_NI | 2023_NI | 2020_Div | 2021_Div | 2022_Div | 2023_Div | 2020_2021_Div_Grow | 2021_2022_Div_Grow | 2022_2023_Div_Grow |
|--------|---------|---------|---------|---------|----------|----------|----------|----------|---------------------|---------------------|---------------------|




**Stalwarts**: 
- Key Information:
  - Year End Data for 5 years (2020-2023)
  - Stock Price 
  - Net Income
  - Net Income Growth
  - PE Ratio
  - GSECTOR
  - Industry Average PE Ratio
  - Market Capitalization

| Ticker | 2023_MarketCap | Market_Cap_Cat | 2023_PE | Gsector    | Avg_PE_Gsector | 2020_NI   | 2021_NI   | 2022_NI   | 2023_NI   | 2020_2021_NI_Grow | 2021_2022_NI_Grow | 2022_2023_NI_Grow |
|--------|----------------|----------------|---------|------------|----------------|-----------|-----------|-----------|-----------|--------------------|--------------------|--------------------|

**Fast Growers**: 
- Key Information:
  - Stock Price
  - Net Income 
  - Net Income Growth Rate 
  
| Ticker | 2020_2021_NI_Grow | 2021_2022_NI_Grow | 2022_2023_NI_Grow | 2023_PE | Average_Growth | Growth_Rate |
|--------|--------------------|--------------------|--------------------|---------|----------------|-------------|
|        |                    |                    |                    |         |                |             |


**Screened Returns Comparison**: 
- Key Information:
  - Stock Price
  - Market Capitalization
  
| Ticker | 2020 (price) | 2020 (market cap) | 2021 (price) | 2021 (market cap) | 2022 (price) | 2022 (market cap) | 2023 (price) | 2023 (market cap) |
|--------|--------------|-------------------|--------------|-------------------|--------------|-------------------|--------------|-------------------|
|        |              |                   |              |                   |              |                   |              |                   |



**Wilshire 5000 % S&P 500 Returns**: 
- Key Information:
  - Stock Price
 
| Ticker | 2020 (price) | 2021 (price) | 2022 (price) | 2023 (price) |
|--------|--------------|--------------|--------------|--------------|
| Wilshire 5000       |              |              |              |              |

| Ticker | 2020 (price) | 2021 (price) | 2022 (price) | 2023 (price) |
|--------|--------------|--------------|--------------|--------------|
| S&P     |              |              |              |              |


#### Data Transformation

**Step 1: Collect data**
- Collect necessary data for creating hollistic Slow Grower, Stalwart, and Fast Grower screening.

**Step 2: Pull Necessary Data From Each Dataset**
    - Clean_Slow_Grow_Master.csv
    - Clean_Stalwart_Master.csv
    - Clean_Fast_Grower_Master.csv

**Step 3: Screen Datasets for Peter Lynch Criterion**
- Screened_Slow_Grow.csv
    - Paid Dividends Every Year?
    - Have Dividends Paid Decreased In Any Year?
- Screened_Stalwart.csv:
    - Company PE Ratio Similar to Industry PE Averages?
    - Has There Been Consistent Net Income Growth?
    - Market Cap IS Large-Cap or Mega-Cap
        - mega-cap: market value of $200 billion or more
        - large-cap: market value between $10 billion and $200 billion;
        - mid-cap: market value between $2 billion and $10 billion;
        - small-cap: market value between $250 million and $2 billion; and
        - micro-cap: market value of less than $250 million.
- Screened_Fast_Grower.csv:
    - Is Net Income Growth Between 20% - 25%?
    - Is The PE Ratio Near the Net Income Growth?

**Step 4: Create a List of Peter Lynch Companies**
- Create a listed of screened Slow Growers, Stalwarts, and Fast Growers.
- Create a dataset which returns their market cap and stock price between 2020-2023.
- Simulate the return of the Peter lynch Screened Companies over that time. 

**Step 5: Create a List of Wilshire 5000 & S&P 500 Returns**
- Create a dataset which returns the Wilshire 5000 stock price between 2020-2023.
- Create a dataset which returns the S&P 500 stock price between 2020-2023.
  
**Step 6: Draw Conclusion**
- Graph the Screened Companies against the returns of the indexes
- Perform more exploration on the screened companies

### Resources
- [Whilshire List](https://info.wilshire.com/Wilshire-5000-Index-Fund-Holdings)
- [One Up On Wall Street](https://yourknowledgedigest.files.wordpress.com/2020/04/one-up-on-wall-street.pdf)
    













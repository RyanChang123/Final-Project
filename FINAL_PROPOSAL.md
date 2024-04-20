# RESEARCH PROPOSAL: Performance of Wilkshire 5000 Firms Screened Through Peter Lynch's Methodology vs. Broader Market

## By Ryan Chang

### Research Question

In this research I am exploring how do firms screened through Peter Lynch's Slow Grower, Stalwart, and Faster Grower methodology compare to the broader market. My hypothesis is that the screened companies will have historically outperform the Wilkshire 5000.

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
   - Compairson to Wilshire return
   - Breakdown of comparison by screening criterion
   - Final conclusion and analysis
 
### Necessary Data

- **One Up On Wall Street**: Peter Lynch's book.
  - **Source:** [One Up on Wall Street](https://yourknowledgedigest.files.wordpress.com/2020/04/one-up-on-wall-street.pdf)
- **Wilshire 5000 Stock List**: Wilkshire 5000 stock list.
  - **Source:**  [Wilshire 5000 List](https://info.wilshire.com/Wilshire-5000-Index-Fund-Holdings)
- **Stock Data**: Key Stock Information.
  - **Source:** Yahoo Finance
- **Wilshire 5000**: Performance from 2021-Present.
  - **Source:** Yahoo Finance

### Final Datasets

**Slow Growers**: 

- Key Information:
  - Year End Data for 5 years (2015-2019)
  - Were Dividends Paid?
  - Dividends Growth Year over Year
  - Dividends Paid as Percentage of Net Income

|         | Year End Data |           |       |
|---------|--------------|-----------|-------|
|         |      "2015-2019"     |         |         |                 
|         | Dividend Amount | Net Income | Dividend Growth |
| Stock   |              |           |       |


**Stalwarts**: 
- Key Information:
  - Year End Data for 5 years (2015-2019)
  - Stock Price 
  - Net Income
  - Net Income Growth
  - PE Ratio
  - CUSIP
  - Inustry Average PE Ratio
  - Market Capitalization

|            | Year End Data |          |         |         |         |         |
|------------|---------------|----------|---------|---------|---------|---------|
|            | "2015-2019"   |          |         |         |         |         |
|            | Price         | Net Income | Net Income Growth | PE Ratio | CUSIP   | Industry PE Ratio | Market Cap |
| Stock      |               |           |                   |          |         |                    |            |

**Fast Growers**: 
- Key Information:
  - Stock Price
  - Net Income 
  - Net Income Growth Rate 
  
|          | Year End Date |          |          |
|----------|---------------|----------|----------|
|         |      "2015-2019"     |         |              
|          | Price         | Net Income | Net Income Growth |
| Stock    |               |          |          |

**Screened Returns Comparison**: 
- Key Information:
  - Stock Price
  - Market Capitalization
  
|          | Year End Date | Market Cap |
|----------|---------------|------------|
|          |    "2020-2023"  |            |
|          | Price         | Market Cap |
| Stock    |               |            |

**Wilshire 5000 returns**: 
- Key Information:
  - Stock Price
 
|          | Year End Date |
|----------|---------------|
|         |      "2020-2023"     |          
|          | Price         |
| Stock    |               |


#### Data Transformation

**Step 1: Prepare and Clean Data**
- Clean the data: Ensure critical columns have no missing values. Remove firms with missing critical values. 

**Step 2: Pull Necessary Data From Each Dataset**
- Slow_Growers.csv
- Stalworths.csv
- Fast_Growers.csv
- Wilshire_return.csv
- Screened_return.csv

**Step 3: Screen Datasets for Peter Lynch Criterion**
- Slow Growers
    - Paid Dividends Every Year?
    - Have Dividends Paid Decreased In Any Year?
    - Dividends Paid Less than 40% of Net Income?
- Stalwarts 
    - Company PE Ratio Lower Than Industy Average?
    - Has There Been Consistent Net Income Growth?
    - Market Cap IS Large-Cap or Mega-Cap
        - mega-cap: market value of $200 billion or more
        - large-cap: market value between $10 billion and $200 billion;
        - mid-cap: market value between $2 billion and $10 billion;
        - small-cap: market value between $250 million and $2 billion; and
        - micro-cap: market value of less than $250 million.
- Fast Growers 
    - Is Net Income Growth Between 20% - 25%?
    - Is The PE Ratio Between 25 - 30?

**Step 4: Create a List of Peter Lynch Companies**
- Create a listed of screened Slow Growers, Stalworts, and Fast Growers.
- Create a dataset which returns their market cap and stock price between 2020-2023.
- Simulate the return of the Peter lynch Screened Companies over that time. 

**Step 5: Create a List of Wilshire 5000 Returns**
- Create a dataset which returns the Wilshire stock price between 2020-2023.

**Step 6: Draw Conclusion**
- Compare the return of the screened companies compared to the return of the index
    - Do this for each screened grouping

### Resources
- [Whilshire List](https://info.wilshire.com/Wilshire-5000-Index-Fund-Holdings)
- [One Up On Wall Street](https://yourknowledgedigest.files.wordpress.com/2020/04/one-up-on-wall-street.pdf)
    













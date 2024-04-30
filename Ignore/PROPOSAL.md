How to screen securities based on Peter Lynch's methodology:

1. Slow Growers ***
2. Stalwarts ***
3. Fast Growers ***

4. Cyclical (not quantitative enough to do)
5. Turnarounds (not quantitative enough to do)
6. Asset Plays (not quantitative enough to do)

What do we want to know or what problems are we trying to solve? As in the midterm, you should list (1) the “bigger” question/debate/problem you’re interested in, and also (2) the specific research question(s) you’ll actually try to answer.

Can utilizing Peter Lynch's investment methodology still work today? If so can we make a stock screener that is able to identify his categorization for Slow Growers, Stalwarts, and Fast Growers? How would an equal weight of these stocks perform against the broader market?

Necessary Data¶
This section should cover:
1. Slow growers
    - 5 years of data for slow-growing companies 
    - Need to know if the company has paid out dividends for every year?
    - Need to know if the company has consistently increased dividends?
    - Need to know what percentage of net income is paid out (provides cushion of company) lower is better
2. Stalwarts 
    - 5 years of data 
    - Need to know the PE ratio of the company compared to the average PE ratio of the industry by year
    - Need to make sure long-term net income has the same growth rate or similar
    - These are large companies need to have a large market cap (most likely mega or large cap) (FINRA)
        - mega-cap: market value of $200 billion or more
        - large-cap: market value between $10 billion and $200 billion;
        - mid-cap: market value between $2 billion and $10 billion;
        - small-cap: market value between $250 million and $2 billion; and
        - micro-cap: market value of less than $250 million.
3. Fast Growers 
    - 5 years of data 
    - Need proper net income growth 
       - Too low 10% - 20%
       - Ideal 20% - 25% 
       - Too high 25% 
    - PE ratio of stock needs to be near the growth rate 

What does the final dataset need to look like (mostly dictated by the question and the availability of data):
    - the final dataset will consist of 5 years of data from all the Wilshire 5000 firms 
    
- For slow growers 
    - Company Name, Ticker, annual dividends over 5 years, Net income over 5 years 
- For stalwarts 
    - Company name, ticker, GICS, Price over 5 years, Current PE, Average GICS PE, Market Cap, Net income for 5 years 
- For Fast Growers
    - Company name, ticker, Net income, Average annual NI growth, Price

What is the sample period?
- 5 years of data 

What are the sample conditions? (Years, restrictions you anticipate (e.g. exclude or require some industries)
- Need to take into consideration the implications from COVID (maybe take data from 2010 - 2015

What variables are absolutely necessary and what would you like to have if possible?
- Company Name, Ticker, annual dividends over 5 years, net income over 5 years, GICS, Price over 5 years, Market Cap

What data do we have and what data do we need?
- Have a list of Wilshire 5000 securities 
- We need all the information listed in the final dataset 

How will we collect more data?
- We will use Yahoo Finance to load the data 

What are the raw inputs and how will you store them (the folder structure(s) for each input type)?
- Raw inputs will be in the inputs folder 

Speculate at a high level (not specific code!) about how you’ll transform the raw data into the final form.
Acknowledgment: We are effectively answering questions 1.1-1.3 and 2.1-2.3 from DS100 in this proposal.

- Need to clean the data and remove all blanks 
- Need to ensure that all the data points are valid and continuous 
- Need to organize data into input folders 
    - one for slow growers
    - one for stalwarts 
    - one for fast growers 
- Need to create an input folder that has all of that information 
- Need to create each of the variables needed based on the input data 
- Finally, need to output a CSV for each highlighting why the companies might fall into each of the categories














# fundamental 
## Dataframe for fundamental financials of multiple stocks
It is a Python 3 library for generating list of stocks' fundamental data through YahooFinance.
The library is primarily based on yfinance package. fundamental requires only list of tickers input from the user and easily generate dataframe for fundamental ratio analysis, relative value ratio analysis and industry relative analysis.

![github](https://user-images.githubusercontent.com/46503526/72200258-4bddb500-3415-11ea-99b2-cde974a7031f.jpg)

## Data inclusion
- financials for recent 3 years. (income statement, balance sheet, cash flow statement)
- calendar year end financials prorated by months
- Trailing twelve months financial by aggregate recent 4 quarters
- Basic share and price for each fiscal year end and recent fiscal quarter end

## Ticker source example
https://www.ishares.com/us/products/239522/ishares-us-technology-etf

- Holding section show the full list of component
- It takes about 10 minutes to create a dataframe for 100 stocks. 

## Usage
```
# down load the py file in the folder

symlist = ['GOOG','MSFT','FB'] 
df = get_df_list(symlist)        

```

## Limitation
- financials are not available from yfinance scraping. 
- slow internet connection would lead scraping error and the program will auto try 3 times. 


# Stocks-Analysis
## Overview of the Project
This project is to analyze 12 stocks' performance in 2017 and 2018 and to uncover which one is promosing for investors. Basically, stocks with higher daily transcation volumes and yearly returns suggest more values and interests for investors. In this project, I will analyze 12 stocks' yearly returns, as well as their total daily transaction volumes in 2017 and 2018. Also, I write two macros for this project and to see whether the refactored one works more efficiently for users. The project will include the result of stock analysis, buying advice, and comparison of two sets of codes.

## Results
### Analysis of Stock Performance
Stocks with positive returns are formated in green while stocks with negative returns are in red. As we can see from the image of the stock performance in 2017, except the stock TERP had a negative yearly return, or a loss, other stocks all increased in values. DQ had the best yearly return, or surged 199.4% in 2017. Other stocks like SEDG, ENPH, FSLR also generated high returns of 184.5%, 129.5%, 101.3% respectively. As for total daily traded volumes, though DQ gained the most in return, it had the least volumes of $35,796,200. SPWR and FSLR had the most volumes of $782,187,000 and $684,181,400, respectively.

![The Stock Analysis in 2017](https://github.com/ZiwenLyu/stocks-analysis/blob/main/2017%20analysis%20result.png)

While looking into the analysis result of all stocks in 2018, we will surprisingly find out that most stocks had negative yearly returns, or declined in values. DQ had the worst return of -62.6%, also stocks like JKS, SPWR, FSLR plummeted 60.5%, 44.6%, and 39.7% in a year. Only two stocks ENPH and RUN survived and generated great profits. ENPH rose 81.9% and RUN rose 84.0%. As for their total volumes, ENPH traded more or $607,473,500 in total.

![The Stock Analysis in 2018](https://github.com/ZiwenLyu/stocks-analysis/blob/main/2018%20analysis%20result.png)


### Buying Suggestions
After the analysis of all stocks in two years, **ENPH** is more likely to generate profits for investors in terms of its good returns in two years and big traded volumes. 


### Results of Applying Two Different Codes
As mentioned, I used two sets of codes to analyze all stocks. Running through the first original script takes much more longer time. As images below shows, running the analysis of all stocks in 2017 takes 1.2s and the 2018 takes 17.3s.

![The orignial script time 2017](https://github.com/ZiwenLyu/stocks-analysis/blob/main/2017%20original%20script%20analysis%20time.png)
![The orignial script time 2018](https://github.com/ZiwenLyu/stocks-analysis/blob/main/2018%20orignial%20script%20analysis%20time.png)

However, the refactored script only uses no more than 0.2s for 2017 stock analysis and 1.5s for 2018 stock analysis. The executation time is much shorter, which means the refactored code is more efficient.

![The refactored script time 2017](https://github.com/ZiwenLyu/stocks-analysis/blob/main/resources/VBA_Challenge_2017.png)
![The refactored script time 2018](https://github.com/ZiwenLyu/stocks-analysis/blob/main/resources/VBA_Challenge_2018.png)


## Summary 

1. Advantages and Disadvantages of refactoring code:

- Advantage: The biggest difference between the original and the refactored code is using a variable as an index to access arrays. In this way, the refactored script doesn't have to use a ***nested For Loop*** that runs an array within another array. It reduces numbers of operations so executing codes becomes easier and more time-saving. 
- Disadvantage: Sometimes each array has different numbers of variables, which means we need to create more variable as indexes for each array and it will also be cumbersome. 

2. Advantages and Disadvantages of applying code to the VBA script:

- Advantages: : This script creates a variable tickerIndex as an index for four arrays: tickers, tickerStaringPrice, tickerEndingPrice, and tickerVolumes, and the four arrays all have 12 variables so using one tickerIndex is really convenient and helpful. It avoids using nested For Loop and saving numbers of operations 12 times than the original one.
- Disadvantages: In my two scripts, the refactored script takes 60 more lines than the origial scripts. 

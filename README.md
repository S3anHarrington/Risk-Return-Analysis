# Analyzing Portfolio Risk and Return

This platform aims to offer clients a one-stop online investment solution for their retirement portfolios that’s both inexpensive and high quality. (Think about Wealthfront or Betterment). To keep the costs low, the firm uses algorithms to build each client's portfolio. The algorithms choose from various investment styles and options.

You've been evaluating four new investment options for inclusion in the client portfolios. Legendary fund and hedge-fund managers run all four selections. to determine the fund with the most investment potential based on key risk-management metrics: the daily returns, standard deviations, Sharpe ratios, and betas.


# Instructions

Import the Data

Use the risk_return_analysis.ipynb file to complete the following steps:

Import the required libraries and dependencies.

Use the read_csv function and the Path module to read the whale_navs.csv file into a Pandas DataFrame. Be sure to create a DateTimeIndex. Review the first five rows of the DataFrame by using the head function.

Use the Pandas pct_change function together with dropna to create the daily returns DataFrame. Base this DataFrame on the NAV prices of the four portfolios and on the closing price of the S&P 500 Index. Review the first five rows of the daily returns DataFrame.


# Analyze the Performance

Analyze the data to determine if any of the portfolios outperform the broader stock market, which the S&P 500 represents. To do so, complete the following steps:

Use the default Pandas plot function to visualize the daily return data of the four fund portfolios and the S&P 500. Be sure to include the title parameter, and adjust the figure size if necessary.

Use the Pandas cumprod function to calculate the cumulative returns for the four fund portfolios and the S&P 500. Review the last five rows of the cumulative returns DataFrame by using the Pandas tail function.

Use the default Pandas plot to visualize the cumulative return values for the four funds and the S&P 500 over time. Be sure to include the title parameter, and adjust the figure size if necessary.


# Analyze the Volatility

Analyze the volatility of each of the four fund portfolios and of the S&P 500 Index by using box plots. To do so, complete the following steps:

Use the Pandas plot function and the kind="box" parameter to visualize the daily return data for each of the four portfolios and for the S&P 500 in a box plot. Be sure to include the title parameter, and adjust the figure size if necessary.

Use the Pandas drop function to create a new DataFrame that contains the data for just the four fund portfolios by dropping the S&P 500 column. Visualize the daily return data for just the four fund portfolios by using another box plot. Be sure to include the title parameter, and adjust the figure size if necessary.

Hint Save this new DataFrame—the one that contains the data for just the four fund portfolios. You’ll use it throughout the analysis.


# Analyze the Risk

Evaluate the risk profile of each portfolio by using the standard deviation and the beta. To do so, complete the following steps:

Use the Pandas std function to calculate the standard deviation for each of the four portfolios and for the S&P 500. Review the standard deviation calculations, sorted from smallest to largest.

Calculate the annualized standard deviation for each of the four portfolios and for the S&P 500. To do that, multiply the standard deviation by the square root of the number of trading days. Use 252 for that number.

Use the daily returns DataFrame and a 21-day rolling window to plot the rolling standard deviations of the four fund portfolios and of the S&P 500 index. Be sure to include the title parameter, and adjust the figure size if necessary.

Use the daily returns DataFrame and a 21-day rolling window to plot the rolling standard deviations of only the four fund portfolios. Be sure to include the title parameter, and adjust the figure size if necessary.



# Analyze the Risk-Return Profile

To determine the overall risk of an asset or portfolio, quantitative analysts and investment managers consider not only its risk metrics but also its risk-return profile. After all, if you have two portfolios that each offer a 10% return but one has less risk, you’d probably invest in the smaller-risk portfolio. For this reason, you need to consider the Sharpe ratios for each portfolio. To do so, complete the following steps:

Use the daily return DataFrame to calculate the annualized average return data for the four fund portfolios and for the S&P 500. Use 252 for the number of trading days. Review the annualized average returns, sorted from lowest to highest.

Calculate the Sharpe ratios for the four fund portfolios and for the S&P 500. To do that, divide the annualized average return by the annualized standard deviation for each. Review the resulting Sharpe ratios, sorted from lowest to highest.

Visualize the Sharpe ratios for the four funds and for the S&P 500 in a bar chart. Be sure to include the title parameter, and adjust the figure size if necessary.



# Diversify the Portfolio

The analysis is nearing completion. Now, you need to evaluate how the portfolios react relative to the broader market. Based on your analysis so far, choose two portfolios that you’re most likely to recommend as investment options. To start your analysis, complete the following step:

Use the Pandas var function to calculate the variance of the S&P 500 by using a 60-day rolling window. Visualize the last five rows of the variance of the S&P 500.
Next, for each of the two portfolios that you chose, complete the following steps:

Using the 60-day rolling window, the daily return data, and the S&P 500 returns, calculate the covariance. Review the last five rows of the covariance of the portfolio.

Calculate the beta of the portfolio. To do that, divide the covariance of the portfolio by the variance of the S&P 500.

Use the Pandas mean function to calculate the average value of the 60-day rolling beta of the portfolio.

Plot the 60-day rolling beta. Be sure to include the title parameter, and adjust the figure size if necessary.

Happy coding!

-----------------------------------------------------------------------

## Contributors

Sean Harrington-
    Linkedin: www.linkedin.com/in/sean-harrington16

-----------------------------------------------------------------------

## License

# Portfolio_Optimization

## Introduction
I have come up with a “Model Portfolio with Multi-cap Investment” approach in the Indian stock markets with weights each for the Large cap, Midcap and Small cap segments and have selected stocks from the corresponding NSE Indexes for Large, Mid and Small cap stocks/scripts. The concepts used are <b>Modern Portfolio Theory</b>, <b>Fama_French Model</b> and <b>CAPM</b>. “MyPortfolio” at any point in time shall consist of ~90% of fund allocation towards stocks (i.e. 20-25 multi-cap multi-sector stocks) and the remaining ~10% in Cash (or liquid instruments) to seize any opportunity that may arise in the markets.

## Modern Portfolio Theory
Modern Portfolio Theory (MPT), a hypothesis put forth by Harry Markowitz in his paper "Portfolio Selection," (published in 1952 by the Journal of Finance) is an investment theory based on the idea that risk-averse investors can construct portfolios to optimize or maximize expected return based on a given level of market risk, emphasizing that risk is an inherent part of higher reward. It is one of the most important and influential economic theories dealing with finance and investment.

Also called "portfolio theory" or "portfolio management theory", Modern Portfolio Theory suggests that it is possible to construct an "efficient frontier" of optimal portfolios, offering the maximum possible expected return for a given level of risk. It suggests that it is not enough to look at the expected risk and return of one particular stock. By investing in more than one stock, an investor can reap the benefits of diversification, particularly a reduction in the riskiness of the portfolio. Modern Portfolio Theory quantifies the benefits of diversification, also known as not putting all of your eggs in one basket.

Consider that, for most investors, the risk they take when they buy a stock is that the return will be lower than expected. In other words, it is the deviation from the average return. Each stock has its own standard deviation from the mean, which Modern Portfolio Theory calls "risk."

The risk in a portfolio of diverse individual stocks will be less than the risk inherent in holding any one of the individual stocks (provided the risks of the various stocks are not directly related). Consider a portfolio that holds two risky stocks: one that pays off when it rains and another that pays off when it doesn't rain. A portfolio that contains both assets will always pay off, regardless of whether it rains or shines. Adding one risky asset to another can reduce the overall risk of an all-weather portfolio.

In other words, Markowitz showed that investment is not just about picking stocks, but about choosing the right combination of stocks among which to distribute one's nest egg.

On the more technical side, there are five statistical risk measurements used in Modern Portfolio Theory (MPT); alpha, beta, standard deviation, R-squared and the Sharpe ratio. All of these indicators are intended to help investors determine a potential investment's risk-reward profile.

## What is Alpha?
Alpha is used in finance as a measure of performance. Alpha, often considered the active return on an investment, gauges the performance of an investment against a market index or benchmark which is considered to represent the market’s movement as a whole. The excess return on an investment relative to the return of a benchmark index is the investment’s alpha. Alpha is used for mutual funds and all types of investments. It is often represented as a single number (like 3 or -5), but this refers to a percentage measuring how the portfolio or fund performed compared to the benchmark index (i.e. 3% better or 5% worse).

Alpha is often used in conjunction with the beta, which measures volatility or risk. Alpha is also often referred to as “excess return” or “abnormal rate of return.”

## What is Beta?
Beta (aka Beta Coefficient) is a measure of the volatility, or systematic risk, of a security or a portfolio in comparison to the market as a whole. Beta is used in the capital asset pricing model (CAPM), which calculates the expected return of an asset based on its beta and expected market returns.

### Calculating Beta
Beta is calculated using regression analysis. Beta represents the tendency of a security's returns to respond to swings in the market. A security's beta is calculated by dividing the covariance the security's returns and the benchmark's returns by the variance of the benchmark's returns over a specified period.

### Using Beta
A security's beta should only be used when a security has a high R-squared value in relation to the benchmark. The R-squared measures the percentage of a security's historical price movements that could be explained by movements in a benchmark index. When using beta to determine the degree of systematic risk, a security with a high R-squared value, in relation to its benchmark, would increase the accuracy of the beta measurement.

### Interpreting Beta
A beta of 1 indicates that the security's price moves with the market. A beta of less than 1 means that the security is theoretically less volatile than the market. A beta of greater than 1 indicates that the security's price is theoretically more volatile than the market. For example, if a stock's beta is 1.2, it's theoretically 20% more volatile than the market.

Here are a beta graphs of a few stocks: 
<img src="./static/Screenshot 2022-09-12 at 18.15.33.png"/>


## What is Standard Deviation?
Standard deviation is a measure of the dispersion of a set of data from its mean. It is calculated as the square root of variance by determining the variation between each data point relative to the mean. If the data points are further from the mean, there is a higher deviation within the data set.

In finance, the standard deviation is a statistical measurement; when applied to the annual rate of return on an investment, it sheds light on the historical volatility of that investment. The greater the standard deviation of a security, the greater the variance between each price and the mean, indicating a larger price range. For example, a volatile stock has a high standard deviation, while the deviation of a stable blue-chip stock is usually rather low.

Here are few volatility graphs:
<img src="./static/Screenshot 2022-09-12 at 18.16.00.png"/>

## What is R-Squared?
R-squared is a statistical measure that represents the percentage of a fund or security's movements that can be explained by movements in a benchmark index.

### BREAKING DOWN R-Squared
R-squared values range from 0 to 1 and are commonly stated as percentages from 0 to 100%. An R-squared of 100% means all movements of a security are completely explained by movements in the index. A high R-squared, between 85% and 100%, indicates the fund's performance patterns have been in line with the index. A fund with a low R-squared, at 70% or less, indicates the security does not act much like the index. A higher R-squared value indicates a more useful beta figure. For example, if a fund has an R-squared value of close to 100% but has a beta below 1, it is most likely offering higher risk-adjusted returns.

## What is the Sharpe Ratio?
The Sharpe ratio is the average return earned in excess of the risk-free rate per unit of volatility or total risk. Subtracting the risk-free rate from the mean return, the performance associated with risk-taking activities can be isolated. One intuition of this calculation is that a portfolio engaging in “zero risks” investment, such as the purchase of U.S. Treasury bills (for which the expected return is the risk-free rate), has a Sharpe ratio of exactly zero. Generally, the greater the value of the Sharpe ratio, the more attractive the risk-adjusted return. The Sharpe Ratio was developed by Nobel laureate William F. Sharpe.

### BREAKING DOWN Sharpe Ratio
The Sharpe ratio has become the most widely used method for calculating risk-adjusted return; however, it can be inaccurate when applied to portfolios or assets that do not have a normal distribution of expected returns. Many assets have a high degree of kurtosis ('fat tails') or negative skewness. The Sharpe ratio also tends to fail when analyzing portfolios with significant non-linear risks, such as options or warrants.

Modern Portfolio Theory states that adding assets to a diversified portfolio that have correlations of less than 1 with each other can decrease portfolio risk without sacrificing return. Such diversification will serve to increase the Sharpe ratio of a portfolio.

### Sharpe ratio = (Mean portfolio return − Risk-free rate) Standard deviation of portfolio return
<img src="./static/Screenshot 2022-09-12 at 18.17.53.png"/>

## Fama And French Three Factor Model
The Fama and French Three Factor Model is an asset pricing model that expands on the capital asset pricing model (CAPM) by adding size and value factors to the market risk factor in CAPM. This model considers the fact that value and small-cap stocks outperform markets on a regular basis. By including these two additional factors, the model adjusts for the outperformance tendency, which is thought to make it a better tool for evaluating manager performance. The three factors are Market Risks, Company Size and Value Factors.

### BREAKING DOWN Fama And French Three Factor Model
Eugene Fama and Kenneth French, both professors at the University of Chicago Booth School of Business, attempted to better measure market returns and, through research, found that value stocks outperform growth stocks. Similarly, small-cap stocks tend to outperform large-cap stocks. As an evaluation tool, the performance of portfolios with a large number of small-cap or value stocks would be lower than the CAPM result, as the Three Factor Model adjusts downward for small-cap and value outperformance.

## Capital Asset Pricing Model - CAPM
The capital asset pricing model (CAPM) is a model that describes the relationship between systematic risk and expected return for assets, particularly stocks. CAPM is widely used throughout finance for the pricing of risky securities, generating expected returns for assets given the risk of those assets and calculating costs of capital.

<img src="./static/Screenshot 2022-09-12 at 18.18.03.png"/>

## Capital Asset Pricing
The general idea behind CAPM is that investors need to be compensated in two ways: time value of money and risk. The time value of money is represented by the risk-free (rf) rate in the formula and compensates the investors for placing money in any investment over a period of time. The risk-free rate is customarily the yield on government bonds like U.S. Treasuries / Treasury bills.

The other half of the CAPM formula represents risk and calculates the amount of compensation the investor needs for taking on additional risk. This is calculated by taking a risk measure (beta) that compares the returns of the asset to the market over a period of time and to the market premium (Rm-rf): the return of the market in excess of the risk-free rate. Beta reflects how risky an asset is compared to overall market risk and is a function of the volatility of the asset and the market as well as the correlation between the two. For stocks, the market is usually represented as the S&P 500 but can be represented by more robust indexes as well.

The CAPM model says that the expected return of a security or a portfolio equals the rate on a risk-free security plus a risk premium. If this expected return does not meet or beat the required return, then the investment should not be undertaken. The security market line plots the results of the CAPM for all different risks (betas).

## Security Market Line
The security market line (SML) is a line drawn on a chart that serves as a graphical representation of the capital asset pricing model (CAPM)—which shows different levels of systematic, or market risk, of various marketable securities, plotted against the expected return of the entire market at any given time.

The security market line is an investment evaluation tool derived from the CAPM—a model that describes risk-return relationship for securities—and is based on the assumption that investors need to be compensated for both the time value of money (TVM) and the corresponding level of risk associated with any investment, referred to as the risk premium.

The formula for plotting the SML is required return = risk-free rate of return + beta (market return - risk-free rate of return).

<img src="./static/Screenshot 2022-09-12 at 22.30.16.png"/>

Here the risk free rate is 8.25% and (market return - risk-free rate of return) is -4.13.

When a security is plotted on the SML chart, if it appears above the SML, it is considered undervalued because the position on the chart indicates that the security offers a greater return against its inherent risk.

Conversely, if the security plots below the SML, it is considered overvalued in price because the expected return does not overcome the inherent risk.


## What Is The Efficient Frontier?
The efficient frontier is the set of optimal portfolios that offers the highest expected return for a defined level of risk or the lowest risk for a given level of expected return. Portfolios that lie below the efficient frontier are sub-optimal because they do not provide enough return for the level of risk. Portfolios that cluster to the right of the efficient frontier are also sub-optimal because they have a higher level of risk for the defined rate of return.

### BREAKING DOWN Efficient Frontier
Since the efficient frontier is curved, rather than linear, a key finding of the concept was the benefit of diversification. Optimal portfolios that comprise the efficient frontier tend to have a higher degree of diversification than the sub-optimal ones, which are typically less diversified. The efficient frontier concept was introduced by Nobel Laureate Harry Markowitz in 1952 and is a cornerstone of modern portfolio theory.

## Optimal Portfolio
One assumption in investing is that a higher degree of risk means a higher potential return. Conversely, investors who take on a low degree of risk have a low potential return. According to Markowitz's theory, there is an optimal portfolio that could be designed with a perfect balance between risk and return. The optimal portfolio does not simply include securities with the highest potential returns or low-risk securities. The optimal portfolio aims to balance securities with the greatest potential returns with an acceptable degree of risk or securities with the lowest degree of risk for a given level of potential return. The points on the plot of risk versus expected returns where optimal portfolios lie are known as the efficient frontier.

## Selecting Investments
Assume a risk-seeking investor uses the efficient frontier to select investments. The investor would select securities that lie on the right end of the efficient frontier. The right end of the efficient frontier includes securities that are expected to have a high degree of risk coupled with high potential returns, which is suitable for highly risk-tolerant investors. Conversely, securities that lie on the left end of the efficient frontier would be suitable for risk-averse investors.

## Selected Stocks in Portfolio:

VOL_UNIONBANK.NS 2.170028 VOL_BANKINDIA.NS 2.113974 VOL_RCOM.NS 1.990837 VOL_CANBK.NS 1.854292 VOL_PCJEWELLER.NS 1.834894 VOL_GMRINFRA.NS 1.766205 VOL_JINDALSTEL.NS 1.524516 VOL_L&TFH.NS 1.444537 """ Volatility Large cap VOL_JPASSOCIAT.NS 4.431737 VOL_GNFC.NS 3.574764 VOL_PNCINFRA.NS 2.278846 VOL_STRTECH.NS 2.229402 VOL_INOXWIND.NS 2.090468 VOL_INFIBEAM.NS 2.008561 VOL_GSFC.NS 1.991663 VOL_RAIN.NS 1.894089 VOL_BBTC.NS 1.829212 VOL_MOIL.NS 1.827504 VOL_FCONSUMER.NS 1.822743 VOL_DBL.NS 1.742365 VOL_ITI.NS 1.710671

## Two Portfolios with Max Sharpe Ratio and Min Volatility

<img src="./static/Screenshot 2022-09-12 at 18.16.32.png"/>


### Portfolio # 1 (Blue star)

Returns 0.250297 Volatility 0.155174 Sharpe Ratio 1.613012 AXISBANK.NS 0.030742 BANKBARODA.NS 0.029452 BHEL.NS 0.003374 HEROMOTOCO.NS 0.003664 CIPLA.NS 0.078108 DRREDDY.NS 0.054943 SBIN.NS 0.025007 HCLTECH.NS 0.070226 RELIANCE.NS 0.106834 HINDUNILVR.NS 0.101651 UNIONBANK.NS 0.101836 BANKINDIA.NS 0.032457 RCOM.NS 0.011342 GMRINFRA.NS 0.014042 JINDALSTEL.NS 0.062114 PCJEWELLER.NS 0.035489 L&TFH.NS 0.068476 JPASSOCIAT.NS 0.023635 GNFC.NS 0.056779 PNCINFRA.NS 0.070353 STRTECH.NS 0.015912 INOXWIND.NS 0.003564

### Portfolio # 2 (Red star)

Returns 0.398010 Volatility 0.197242 Sharpe Ratio 2.017875 AXISBANK.NS 0.087238 BANKBARODA.NS 0.003753 BHEL.NS 0.055004 HEROMOTOCO.NS 0.016172 CIPLA.NS 0.014446 DRREDDY.NS 0.012755 SBIN.NS 0.075367 HCLTECH.NS 0.070347 RELIANCE.NS 0.002490 HINDUNILVR.NS 0.009251 UNIONBANK.NS 0.097322 BANKINDIA.NS 0.010150 RCOM.NS 0.000398 GMRINFRA.NS 0.029947 JINDALSTEL.NS 0.069755 PCJEWELLER.NS 0.080285 L&TFH.NS 0.088866 JPASSOCIAT.NS 0.005632 GNFC.NS 0.093626 PNCINFRA.NS 0.070391 STRTECH.NS 0.105415 INOXWIND.NS 0.001390


PORTFOLIO BETA= 1.30107342631
PORTFOLIOALPHA= 0.224494080754
PORTFOLIOVOLATILITY= 0.228721920896
MOMENTUM= 0.28839782936

## Data Analysis based on the output from EFFICIENCY FRONTIER OF MYPORTFOLIO STOCKS MYPORTFOLIO – with a combination of Multi-Cap stocks provides the Investor with two options:

1) Relatively Lower Risk with Moderate Return which has a Portfolio Return of 25% with Volatility of 15% and Portfolio Sharpe Ratio of 1.61

2) Relatively Higher Risk with Higher Returns which has a Portfolio Return of 39% with Volatility of 19% and Portfolio Sharpe Ratio of 2.01

Based on the risk profile of the Investor, he/she may choose to go with either of portfolio 1 or 2 for Investment purposes.

## Key Findings
Summarizing the above-mentioned steps, Quantitative Finance techniques help:

1) Identify Beta values for Large, Mid and Small Cap Stocks
2) Identify Volatility values for these stocks
3) Back Testing of the Index with stocks and performance over 8 years period
4) Help arrives at a set of stocks that could constitute MyPortfolio (max of 25 stocks)
5) Determine the weights to be provided to each stock in the basket/portfolio
6) Determine the Efficiency Frontier for 2 portfolios based on backtesting for 2 years
7) Provide Options to the Investor depending on the Risk Profile, with a guidance around Expected Returns, Volatility and Sharpe Ratio of the underlying two portfolios with stock weights

# Introduction
The global financial crisis of 2008 was a pivotal event in the history of financial markets. It reshaped the global economy, with banks and financial institutions at the epicenter of the turmoil. This project aims to explore how major U.S. bank stocks performed before, during, and after the crisis, providing insights into their recovery and resilience. By focusing on the stock prices of some of the largest financial institutions, we can gain a better understanding of the impact the crisis had on the banking sector, as well as how these banks rebounded in the following years.

The analysis will focus on the stock performance of six key banks:

- Bank of America
- CitiGroup
- Goldman Sachs
- JPMorgan Chase
- Morgan Stanley
- Wells Fargo
  
This study will serve as a way to track the trajectory of these banks during a period of extreme volatility and uncertainty, from the crisis up until late 2023.

# Overview
In this exploratory data analysis (EDA), we will gather historical stock price data for the selected banks from 2006 to 2016. By utilizing this data, we will perform the following:

- Data Collection: We will extract the stock price data using APIs such as pandas_datareader, which will allow us to pull historical data from reliable sources like Yahoo Finance.

- Data Visualization: Through visualizations such as time-series plots, rolling statistics, and correlation heatmaps, we will explore the general trends of these stocks and any significant events that influenced their behavior.

- Crisis Analysis: Special emphasis will be placed on analyzing how these stocks behaved during the 2008 financial crisis, identifying sharp declines and recovery patterns.

- Comparison of Banks: By comparing stock performance across different banks, we will identify which institutions were more resilient and which struggled, drawing insights into their risk management and business models.

- Trend Analysis Post-Crisis: We will also explore the performance of these banks from 2009 to early 2016, providing insights into their recovery, growth, and any external factors that may have influenced their stock prices.

Through this analysis, we hope to understand the broader market dynamics and the specific impacts on individual banks. By leveraging historical data and conducting thorough visual and statistical analysis, we aim to draw meaningful conclusions about the financial crisis's effects on the banking sector and their subsequent recovery.

# Let's get started

### The Imports

![The Imports](https://github.com/user-attachments/assets/35045801-4f0f-4c37-839d-eb57b0d26caa)

### Getting_Data
![Getting_Data](https://github.com/user-attachments/assets/f008ff11-55ba-4ac5-8008-23d7ee064f4e)

### Check Data
![Check_Data](https://github.com/user-attachments/assets/91ac92a2-71cb-41d1-90fe-3e4f48528856)

## Exploratory Datra Analysis
``
 ![EDA1](https://github.com/user-attachments/assets/2577e3c7-84f4-4949-92f2-c4054f6f2ea6)

#### Insight
 Goldman Sachs (GS) had the highest closing price of 423.85, followed by JPMorgan(JPM) at 171.78. Citigroup (C) and Bank of America (BAC) had similar closing prices centered aroung mid-50s.

 ![EDA2](https://github.com/user-attachments/assets/2ec16bd2-39cb-48c5-a0ec-9d55518dec78)
![EDA3](https://github.com/user-attachments/assets/33863608-6e21-4e24-8235-b77774024164)

#### Insight:

- Volatility of Citigroup: The returns available on Citigroup Global Markets stocks are more volatile and have a higher extreme value in time than other banks probe in this research. This may be explained due its investments in risky assets or incurring larger than normal losses in times of financial crises caused during this period (the year of the 2008 financial crises). A greater spread in the distribution of winning trades is attributed to Citigroup with the frequent incidence of red trades judging from the KDE.

- Positive Correlations: The majority of the banks also tend to have very strong return correlations, indicating that their stock returns bounce back or fall at the same time. This is mostly so, as majority of the banks will be under the influence of comparable macroeconomic factors such as (but not limited to): interest rates, market factors, and regulatory settings.

- Citigroup vs Other Banks: Out of the rest, including JPM, BAC and GS, Citigroup seems to deviate from the typical market trend most of the time. When the scatter plots of the other wholesale banks group were constructed each point tends to cluster a given line while with Citigroup the pattern is wider with more points away from the cluster which suggests greater sensitivity of the bank.

  ![EDA4](https://github.com/user-attachments/assets/91987aca-0fbc-4719-9c58-9a6696007214)

  #### Insight
- ##### Worst Single-Day Drop (via returns.idxmin()):
 

Four banks suffered sharp declines in their popularities in the stock market on January 20, 2009 (On the day of President Obama’s Inauguration). The establishments in focus were: 
 
BAC (Bank of America) 

JPM (JPMorgan) 
 
MS (Morgan Stanley) 
 
WFC (Wells Fargo) 
 
This mass fall could possibly imply a reaction to very significant economic news, such as that there were concerns around that time over the broader financial crisis appearing, or usually it is the change of political party and the leadership. 
 
 #### Best Single-Day Gain (via returns.idxmax()): 
As some of those notable dates include:  

- BAC had its best day on 9 April 2009. 

- C (Citigroup) had a stock split in May 2011 which alter the returns than another mad on November 24, 2008.

There was a big jump in the stock price of JPM on January 21, 2009 the day after the inauguration.

Most of these drastic jumps can usually be accounted to the change of mood of the investors or news/events in the market. 
 
 #### Standard Deviation Analysis (Volatility):
  
- ##### Overall Period (via returns.std()):

It is interesting to note that Citigroup (C) has been classified as the riskiest bank over the whole period since it obtained the highest standard deviation 0.032251, suggesting riskier level of its stock’s returns where its volatility is high.

2023 Specific Period (via .loc["2023-01-01":"2023-12-31"].std.))

In the year Wise (WFC) faced the stiffest competition with the maximum risk in terms of volatility (0.017460). This indicates that wells fargo & co sec exhibited the highest degree of variability.

``


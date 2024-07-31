# Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds
This project analyzes the performance of small, mid, and large cap funds from 2020 to 2023. Using linear regression, it calculates volatility and risk-adjusted returns based on closing indices data, providing insights into each fund's risk and performance.
## Objectives:
So, as we know in 2020 due to COVID-19 and in 2022 due to Russia-Ukraine war Indian stock market went through a deep red. It fell sharply. Although it recovered but as an stock market enthusiast I decided to analyze their perfomance from the start of 2020 to end of 2023. My main motive was to draw a quantitative view about how each of these funds reacted during thet period of time and in the end which gave a better returns taking volatility into account. 
Starting with the data source, here for this project I collected all 4 year data of small, mid and large cap funds from  https://www.bseindia.com/Indices/IndexArchiveData.html this website. I only considered their closing price of each day. Total 994 days of data was there.
## Data Visualization:
![image](https://github.com/daniketdas/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/44a19175-4247-4018-a157-7e729e490031) **This graph presents their performance over 4 years.**
## Evaluating rewards using Linear Regression:
Then I used Linear Regression method to quantify their returns/reward over 4 years.

![image](https://github.com/daniketdas/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/d56d38ca-4409-4ba5-82f4-c1af22b7eac2) 
![image](https://github.com/daniketdas/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/f25b5196-c83e-474f-ae04-2a864eda505a) 

**Here I got intercept parameter and coefficients for all the funds, where each fund has been taken as both independent and dependent variable.**


![image](https://github.com/daniketdas/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/ddaf6b6f-27c1-45a3-bd2c-69db7e9fc00e) 
![image](https://github.com/daniketdas/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/c2802d32-057d-44dc-acf9-a572243137ea)

**So these are the residuals for each of the cases. Which represents how much the predicted value of each funds deviates from the actual value.**

![image](https://github.com/daniketdas/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/a49934f7-e980-486c-be19-cec260b9ade3)

**This is the correlation between funds.**

![image](https://github.com/daniketdas/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/d985a943-3f4c-404d-acaf-e15aaed57a62)

**This the reward of each of the funds, which I got from the sumproduct of residual percentage and correlation.**
## Volatility Measurement:
![image](https://github.com/daniketdas/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/fc63d1e4-8a83-4219-9bf5-969f6d54f2be)

**This shows the volatility of 3 funds.**

To get this first I calculated their per day percentage change in their points from previous day and then got standard deviance of that. Then multiplied sqrt of 252 with standard devance to get volatility of each fund.
## Evaluating Risk-Adjusted reward of all funds:
![image](https://github.com/daniketdas/Quantitative-Analysis-of-Fund-Performance-Risk-Adjusted-Returns-for-Small-Mid-and-Large-Cap-Funds/assets/162815966/0746c841-4837-4dfd-aae5-20e70561a559)

**This shows the risk-adjusted-reward of small, mid and large cap funds.**

This involves dividing the reward by volatility.

## Result:
 * This suggests that mid cap funds offered the most favorable balance of risk and reward of 0.22, making them an attractive option for investors seeking optimized returns relative to their risk exposure.
 * Small cap funds showed lower risk-adjusted return than mid-cap. Although small cap funds usually give higher returns due to their small market cap and high growth rate but in this period it fell short of mid cap when risk considered as it showed much volatility as compared to mid cap.
 * Large-cap funds showed a negative risk-adjusted reward of -0.19. This result indicates that, over the analysed period, large-cap funds did not provide adequate returns relative to the risks involved.








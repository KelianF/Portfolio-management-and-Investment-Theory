# Introduction


## Calculating returns

There are two commonly used methods to calculate price changes, or returns.

Log returns:

![equation](https://latex.codecogs.com/svg.latex?R_t=ln(P_t+D_t)-ln(P_{t-1}))

Arithmetic returns:
![equation](https://latex.codecogs.com/svg.latex?R_t=\frac{P_t+D_t-P_{t-1}}{P_{t-1}})

Where ![equation](https://latex.codecogs.com/svg.latex?D) is the dividend (if any).

(Semi-)Riskless Assets

For some assets, the return is known for certain, there is no risk involed. This existence of certainty implies that the investor can associate a certain payoff with each investment. One example of such asset is a Treasury Bill (T-Bill), by which the return is guaranteed by the government. Within the literature such asset is called a risk free rate of return (![equation](https://latex.codecogs.com/svg.latex?R_f))

Risky Assets

It is often desirable to monitor financial price behaviour frequently and try to understand the probable development of prices in the future. Statistical methods are used to understand how prices behave. Using past prices to estimate the expected values of future distribution has represented a problem for many researchers. This usually produced the suimple forecast that the best estimate of tomorrow's price is today's price. Stock prices are said to follow a random walk. Direct statistical analysis of financial prices is difficult, because consecutive prices are highly correlated and the variance of prices increase with time. Hence, returns rather than prices are usually studied.

For most assets the existence of risk implies that the payoff must be described by a set of outcomes/returns and their associated probability of occurence called return distribution.

one of the statistic to represent this distribution is the expected return (![equation](https://latex.codecogs.com/svg.latex?E(R))) :

![equation](https://latex.codecogs.com/svg.latex?E(R)=\sum_{j=1}^{N}P_jR_j)

Where ![equation](https://latex.codecogs.com/svg.latex?R) is the actual return, ![equation](https://latex.codecogs.com/svg.latex?N) is the number of possible outcome and ![equation](https://latex.codecogs.com/svg.latex?P) is the probability of the return j on the asset.

Expected return is also called the Mean, or the average in statistics.


Properties of returns:

![equation](https://latex.codecogs.com/svg.latex?E(R_{1i}+R_{2i})=E(R_{1i})+E(R_{2i}))

![equation](https://latex.codecogs.com/svg.latex?E(c(R_i))=cE(R_i))  ; with c is a constant

![equation](https://latex.codecogs.com/svg.latex?var(R_{1i}+R_{2i})=var(R_{1i})+var(R_{2i})+2cov(R_{1i}R_{2i}))

![equation](https://latex.codecogs.com/svg.latex?var(c(R_1}))=c^2var(R_1))

![equation](https://latex.codecogs.com/svg.latex?var(aR_{1}+bR_{2})=a^2var(R_1)+b^2var(R_2)+2abCov(R_1+R_2))


Summary statistics of Returns

In practice the distribution of the outcomes will not be known. The number of events is just the sample size N and the probability of an event is equal at ![equation](https://latex.codecogs.com/svg.latex?\frac{1}{N})

It is easier to represent the possible outcomes by summary measures such as:

- Mean

- Standard Deviation, Variance, Mean Absolute Dispertion, Semivariance

- Skewness

- Kurtosis

- Autocorrelation coefficient


The Mean of Returns

Average or mens are calculated as:

![equation](https://latex.codecogs.com/svg.latex?R=\frac{1}{N}\sum_{t=1}^{N}R_t)

With N the number of observation. The averages for each period can be very small and they can be easier to interpret if we consider returns over one year.














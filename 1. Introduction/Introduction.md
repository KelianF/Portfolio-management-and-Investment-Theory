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

The historic annual compound rate ![equation](https://latex.codecogs.com/svg.latex?G) giving the same return after ![equation](https://latex.codecogs.com/svg.latex?\frac{N}{T}) years is definedby:

![equation](https://latex.codecogs.com/svg.latex?(1+G)^{1/N}=\exp{NR})

![equation](https://latex.codecogs.com/svg.latex?\frac{N}{T}ln(1+G)=NR)

![equation](https://latex.codecogs.com/svg.latex?ln(1+G)=TR)

![equation](https://latex.codecogs.com/svg.latex?G=\exp{TR}-1)

Standard Deviation of Returns

The standard deviation is the most commonly used measure of volatility of a time series. In finance it is used as a measure of risk.

It is calculated as:

![equation](https://latex.codecogs.com/svg.latex?\sigma=(\frac{1}{N-1}\sum_{t=1}^N(R_t-R)^2)^0.5)

The variance is the second most commonly used measure of volatility:

![equation](https://latex.codecogs.com/svg.latex?\sigma^2=(\frac{1}{N-1}\sum_{t=1}^N(R_t-R)^2))

Mean absolute Dispersion of Returns

![equation](https://latex.codecogs.com/svg.latex?MAD=\frac{1}{N-1}\sum_{t=1}^N|R_t-R|)

Semi-Variance of Returns

It is used to measure returns, however it only takes into account negarive returns.

![equation](https://latex.codecogs.com/svg.latex?SV=\frac{1}{N-1}\sum_{t=1}^N(R_t-R)^2) if ![equation](https://latex.codecogs.com/svg.latex?(R_t-R)<0)

Skeyness of returns

Skewness statistics are used to assess the symmetry of the distribution.

![equation](https://latex.codecogs.com/svg.latex?SKEW=\frac{1}{N-1}\sum_{t=1}^N\frac{(R_t-R)^3}{\sigma^3})

If the returns are from a normal distribution the the skewness should be equal to 0.
The standard error of the Skewness is equal to ![equation](https://latex.codecogs.com/svg.latex?(\frac{3}{N})), and this standard error is valid to use if the sample is from a normal distribution.

Kurtosis of the Returns

Kurtosis statistic is used to assess the thickness of the tails of the distribution.

![equation](https://latex.codecogs.com/svg.latex?KURT=\frac{1}{N-1}\sum_{t=1}^N\frac{(R_t-R)^4}{\sigma^4})

If the returns are from a normal distribution the Kurtosis should be equal to 3. High value of Kurt means fatter tails. 

Autocorrelation of Returns

The correlation between returns separated by a lag of ![equation](https://latex.codecogs.com/svg.latex?\tau) is used to measure persistence and is calculated by the sample correlation coefficient: 

![equation](https://latex.codecogs.com/svg.latex?\rho_{\tau}=\frac{\sum^{N-\tau}_{t=1}{(R_t-\bar{R})(R_{t-\tau}-\bar{R})}}{\sum^N_{t=1}{(R_t-\bar{R})^2}})

The null hypothesis of no serial correlation (white noise) can be tested using the ljung-box Q-statistic:

![equation](https://latex.codecogs.com/svg.latex?Q=N(N+2)\sum_{j<M}{\frac{1}{N-j}}\rho^2_j) 
; With ![equation](https://latex.codecogs.com/svg.latex?Q\sim\chi^2(M))
and ![equation](https://latex.codecogs.com/svg.latex?M) the number of lags chosen


Portfolio Return

The expected return on a portfolio of asset is simply the weighted average of the expected returns on the individual assets:

![equation](https://latex.codecogs.com/svg.latex?E(R_p)=\sum^N_{i=1}{R_i})

Thus the mean return on a portfolio of assets is simply the weighted average of the mean return on the individual assets:

![equation](https://latex.codecogs.com/svg.latex?\bar{R}_p=\sum^N_{i=1}{X_i\bar{R}_i})


Portfolio Risk

![equation](https://latex.codecogs.com/svg.latex?\sigma_p=(\sum^N_{i=1}{X^2_i\sigma^2_i}+\sum^N_{i=1}{\sum^N_{j=1}{X_iX_j\sigma_{ij}}})^{\frac{1}{2}})

The correlation between two assets is related to the covariance

![equation](https://latex.codecogs.com/svg.latex?-1<\rho_{ij}=\frac{\sigma_{ij}}{\sigma{i}\sigma{j}}<1)

It is possible to reduce risk by adding more assets to a portfolio. 
However, it is possible to ask the question: would it be possible to reduce the risk to zero by adding enough assets?

We have the risk of a portfolio:

![equation](https://latex.codecogs.com/svg.latex?\sigma^2_p=\frac{1}{N}\sum^N_{i=1}{\frac{\sigma^2_i}{N}}+\frac{N-1}{N}\sum^N_{i=1}\sum^N_{j=1}{\frac{\sigma_{ij}}{N(N-1)}})

![equation](https://latex.codecogs.com/svg.latex?\sigma^2_p=\frac{1}{N}\bar{\sigma}^2_i+\frac{N-1}{N}\bar{\sigma}_{ij})

= individual risk + covariance risk

As ![equation](https://latex.codecogs.com/svg.latex?N\rightarrow\inf) then ![equation](https://latex.codecogs.com/svg.latex?\sigma^2_p\rightarrow\bar{\sigma}_{ij})

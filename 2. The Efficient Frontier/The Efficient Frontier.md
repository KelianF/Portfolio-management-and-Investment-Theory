# The Efficient Frontier

## Expected return and risk on a two asset portfolio

The Minimum Variance Frontier shows the minimum risk for a given expected return. In order to derive the minimum variance we need to examine all feasable combinations of assets in excpected return and risk space.

For simplicity, we shall start with  a two asset portfolio.

![equation](https://latex.codecogs.com/svg.latex?\bar{R}_p=X_1R_1+X_2R_2)

![equation](https://latex.codecogs.com/svg.latex?\sigma^2_p=X_1^2\sigma_1^2+X_2^2\sigma_2^2+2X_1X_2\sigma_1\sigma_2\rho_{12})

## The minimum Variance Frontier

Assuming ![equation](https://latex.codecogs.com/svg.latex?1=X_1X_2), this implies a non linearity between ![equation](https://latex.codecogs.com/svg.latex?R_p) and ![equation](https://latex.codecogs.com/svg.latex?\sigma_p).

This gives us:

![equation](https://latex.codecogs.com/svg.latex?X_1=\frac{R_p-R_2}{R_1-R_2})

This gives us the hyperbola formula:

![equation](https://latex.codecogs.com/svg.latex?\sigma_p^2=\frac{R_p-R_2}{R_1-R_2}^2\sigma_1^2+(1-\frac{R_p-R_2}{R_1-R_2})^2\sigma^2+2(\frac{R_p-R_2}{R_1-R_2})(1-\frac{R_p-R_2}{R_1-R_2})\sigma_1\sigma_2\rho_{12})

with: ![equation](https://latex.codecogs.com/svg.latex?\sigma_p=[X^2_1\sigma^2_1-(1-X_1)^2\sigma^2_2+2X_1(1-X_1)\sigma_1\sigma_2\rho_{12}]^2)

It is possible to find what the Xi are that achieves minimum risk by differentiating ![equation](https://latex.codecogs.com/svg.latex?\sigma_p) with respect to ![equation](https://latex.codecogs.com/svg.latex?X1) and solve it.

![equation](https://latex.codecogs.com/svg.latex?\frac{\partial\sigma_p}{\partial{X_1}}=\frac{\sigma^2}{2}[2X^2_1\sigma^2_1-2\sigma^2_2+2X_1\sigma^2_2+2\sigma_1\sigma_2\rho_{12}-4X_1\sigma_1\sigma_2\rho_{12}]=0)

So:

![equation](https://latex.codecogs.com/svg.latex?X_1=\frac{\sigma^2_2-\sigma_1\sigma_2\rho_{12}}{\sigma^2_1+\sigma^2_2-2\sigma_1\sigma_2\rho_{12}})

This gives us four equations to examine a two asset portfolio, the first three present a relationship between risk and return:

![equation](https://latex.codecogs.com/svg.latex?R_p=X_1R_1+X_2R_2)

![equation](https://latex.codecogs.com/svg.latex?\sigma^2_p=X_1^2\sigma_1^2+X_2^@\sigma_2^2+2X_1X_2\sigma_1\sigma_2\rgo_{12})

![equation](https://latex.codecogs.com/svg.latex?1=X_1X_2)

the foourth equation allowing to work out the portfolio on the minimum variance frontier that has minimum variance of all portfolio:

![equation](https://latex.codecogs.com/svg.latex?X_1=\frac{\sigma_2^2-\sigma_1\sigma_2\rho_{12}}{\sigma_1^2+\sigma_2^2-2\sigma_1\sigma_2\rho_{12}})

Hence, it is possible to draw the minimum variance frontier for different values of the inputs (the means, variance and correlation among returns).

In case the correlation between the returns is of 1, the volatility of the portfolio becomes:
![equation](https://latex.codecogs.com/svg.latex?\sigma_p=X_1\sigma_1+(1-X_1)\sigma_2)

If the correlation of returns is -1 then:

![equation](https://latex.codecogs.com/svg.latex?\sigma_p=-X_1\sigma_1+(1-X_1)\sigma_2)
Since risk is always positive, there is always a unique solution. Risk is at minimum when:  ![equation](https://latex.codecogs.com/svg.latex?X_1=\frac{\sigma_2}{\sigma_1+\sigma_2}).

When the correlation is equal to 0, then:
![equation](https://latex.codecogs.com/svg.latex?\sigma_p=[(\sigma_1^2+\sigma_2^2)^2X_1^2-2\sigma_2^2X_1+\sigma_2^2]^{\frac{1}{2}})

## The shape of the Minimum Variance Frontier

The efficient frontier gives maximum return for a given risk. Assuming Short seeling is permited, this allows the efficient frontier to extens infinitely on the right hand side.
Furthermore, if investors can borrow at a risk free rate of interest  ![equation](https://latex.codecogs.com/svg.latex?r_f)  this translates as the begining of the efficient frontier commencing on this point of reference on the left hand side.

## The transformation line

Let the relationship between  ![equation](https://latex.codecogs.com/svg.latex?E(R_p))  and ![equation](https://latex.codecogs.com/svg.latex?\sigma_p)  be represented as below:

![equation](https://latex.codecogs.com/svg.latex?E(R_p)=r_f+[\frac{E(R_A)-r_f}{\sigma_A}]\sigma_p)

This is the equation of a line. As obviously represented the intercept is the risk free rate, and the coefficient is the sharpe ratio.

The interesting goal here is to find the tangency point between the transformation line and the minimum variance frontier when only risky assets are included. This is an optimizing problem which aims at maximizing returns for a given risk. Indeed this does not give only one point but a range of points called the efficient frontier, which depends on the risk appetite.


## Risk Aversion

Forecasting risk aversion or seekness would be an incommensurable task, however understanding past risk taste could represent important information. 

Defining Expected Utility from N outomes as:


![equation](https://latex.codecogs.com/svg.latex?E(U)=\sum_{i=1}^{N}P(W_i)U(W_i))

With P the probability of an outcome.

Now knowing this, one of the measure of risk aversion can be introduced: Absolute Risk Aversion.

![equation](https://latex.codecogs.com/svg.latex?ARA(W)=-\frac{U"(W)}{U'(W)})

If an investor decrease the amount invested as wealth increases, the investor is said to show increasing absolute risk aversion, ARA'(W)>0. In the oposite side, it would be said to show decreasing absolute risk aversion ARA'(W)<0


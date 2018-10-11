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

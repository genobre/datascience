# Statistical Learning Approach

In this section we are going to talk about the statistical approach to predict a time series. The codes are available in the folder codes.

## Random Walk

A Random Walk model is one where the value at a given time $(y_t)$ is the value at the previous time $(y_{t-1})$ plus a random noise, that is normally distribuited (with mean of 0 and variance of 1). 

Therefore, the formula for the Random Walk is:

$$ X_{t} = X_{t-1} + Z_{t} $$

If we substitute $X_{t-1}$ with its respective formula and so on, we end up with the following:

$$ X_{t}=\sum_{i=1}^{t} Z_{i} $$

Below we can see an example of a simulated Random Walk:

![Random Walk](../00_images/randomwalk.png)

The ACF of the Random Walk Model looks like the following:

![ACF Random Walk](../00_images/ACFRandomWalk.png)

We can see that the autocorrelation starts very high and slowly goes down. That is an indicative of a trend. If we want to remove that trend, we can differenciate the series to get only the noise. If we do that, we get the following result:

![Random Walk Noise](../00_images/randomwalknoise.png)

We can see now that there is no clear trend in the series and we have purely the noise. To make sure of that, we can also see the ACF of the difference:

![Noise ACF](../00_images/ACFnoise.png)

In the Jupyter Notebook [randomwalk.ipynb](./codes/randomwalk.ipynb) you can see the steps to simulate a Random Walk, plot its correlogram, differenciate and then see the ACF of the difference.

## Moving Average Model 

Rather than using past values of the forecast variable in a regression, a Moving Average Model uses past errors in a regression-like model

## Autoregressive Model

## ARMA: Autoregressive Moving Average Model

## ARIMA: Autoregressive Integrated Moving Average

## SARIMA

## AIC: Akaike Information Criterion

## SARIMAX

## VAR: Vector Autoregressions

## VARMA: Vector Autoregressions Moving Average

## VARMAX: 
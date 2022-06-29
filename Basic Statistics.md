Description: A breakdown of basic statistics and its notation.

# Basic Statistics

### What is the bernoulli and binomial distribution ?

Bernoulli distribution: The random variable can either be 0 or 1. 
Binomial distribution: The random variable remains to have only two states, this shows the probability of measuring either state x number of times given n independent occurrences.

### What is the mean, expectation and standard deviation?

The mean is the frequency of each value occurring, multiplied by the value all summed for each random variable.

$\overline{x} = 1/n(\Sigma fx)$

The expectation is the probability of each value multiplied by the value, summed for all values. This is the value the mean tends to as the sample size increases.

$E(x) = \Sigma x P(X=x)$

The variance is the average of the squared difference from the mean.

$\sigma^2 = E(X^2) - (E(X))^2$

The standard deviation is the square root of the variance, showing essentially the average distance from the mean.

$\sigma$

An overall shift to all data points will effect expectation and not variance:

$E(X \pm a) = E(X) \pm a$

$Var(X \pm a) = Var(X)$

An overall multiplier to all data points effects both expectation and variance:

$E(aX) = aE(X)$

$Var(aX) = a^2Var(X)$

## Poisson Distribution

- Random discrete variable is a count of the number of events occurring at random in regions of time and space.
  - All events are independent 
  - No two events at the same time
  - Over a short period of time or on a small region the probability is the same

$p_x = P(X=x) = e^-\lambda *\lambda^x/x!$ 

Recurrence formula:

$P(X=x) = \lambda/x * P(X= x-1)$

$\lambda$ is the mean var and $\sqrt(\lambda)$ is the std

95% of values are between the mean $\pm$ 2 std

Independent Poisson random variables can be added to give another Poisson random variable

## Continuos variables

Discrete variables are a known list of possible numbers

Continuos random variables are infinite.

The relative frequency density; is a measurement of the relative frequency over a class width (interval between two values) 

$\frac{Relative frequency}{class width} = Relative frequency density$

The probability density function f(x); is the relative frequency density as n increases and the class width decreases

Area under a plotted f(x) gives the probability for that range of continuos variables.

$P(X<x) = \int_{-\infin}^{x} f(x)$

$\frac{d}{dx}P(X<x) = f(x)$

You cannot get the probability for a specific value via f(x):

$P(X=k) = 0$

### Median

The median value (m) is when the probability for values above and below are 0.5. 

$\int_{m}^{\inf} f(x) = 0.5$

### Percentile

The Xth percentile is the value below which the probability is X/100:

90th percentile

$P(X<x_{90th}) = 0.9$

### Mean

If assume the a small width of delta x, the mean will be $\sum x(f(x)\delta(x))$ (the brackets give the probabilty and multiplying by x gives the mean). As delta x tends to 0 this becomes:

$\bar{x} = \int xf(x)$

The population mean is then :

$\mu = \int_{-\infty}^{\infty} xf(x) dx$

The variance is:

$Var(x) = \int_{-\infty}^{\infty} (x -\mu)^2 f(x) dx$

## Estimation

### Confidence Interval

**Normal distribution** : Data set centered evenly about a value, giving a bell curve.

To calculate the confidence interval of a population mean, use the variable Z below, where $\bar{X}$ is variable corresponding to the sample mean:

$Z = (\bar{X} - \mu)/ (\sigma/ \sqrt{n}$)

For a normal distribution with mean 0 and std of 1 N(0,1) the confidence interval is:

$(\bar{x} - 1.96 (\sigma/\sqrt{n}),\bar{x} - 1.96 (\sigma/\sqrt{n}))$

The above interval on an average of 95% of the time will include the mean.

### T Distribution

If the the sample size is limited and below 30, then instead of a normal and T distribution is used.

A T dist has degrees of freedom (v) = n-1:

- A normal distribtion has degrees of freedom v = $\infty$
- n being the sample size

If the variance is unknown and n is large, Z can be adjusted to use s^2 which is an unbiased estimate of the variance. This gives two random variables in the equation X and S:

  $T = (\bar{X} - \mu)/ (S/\sqrt{n})$

c is the critical value depending on the distribution parameters and the confidence interval required:

$(\bar{x} - c(s\sqrt{n}),\bar{x} - c(s\sqrt{n}))$
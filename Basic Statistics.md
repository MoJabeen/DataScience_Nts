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

- Random variable is a count of the number of events occurring at random in regions of time and space.
  - All events are independent 
  - No two events at the same time
  - Over a short period of time or on a small region the probability is the same

$p_x = P(X=x) = e^-\lambda *\lambda^x/x!$ 

Recurrence formula:

$P(X=x) = \lambda/x * P(X= x-1)$

$\lambda$ is the mean var and $\sqrt(\lambda)$ is the std

95% of values between the mean $\pm$ 2 std

Independent Poisson random variables can be added to give another Poisson random variable

# weibull-ml-parameters
Max likelihood estimation for Weibull distribution parameters

The following data are originating from a Weibull distribution:
3,35  1,46  2,84  1,06  0,74  5,27  2,4  1,01  2,31  2,66

The probability density function of a Weibull distribution is:

$$ f(x, \lambda, k) = \frac k\lambda * (\frac x \lambda ) ^{k-1} e^{{(-x/\lambda)}^k}$$

if $x \geq 0 $ , otherwise 0.

The $\lambda$ is the scale parameter, k is the shape parameter.

The Maximum Likelihood estimation of the parameters:
$$ \lambda_{ML} = \frac{\sum^n_{i=1}x^{k}_{i}log x_{i}}{\sum^n_{i=1}x^{k}_{i}} - \frac{1}{k} - \frac{1}{n}\sum^{n}_{i=1}log x_{i} = 0 $$

The task is to use a null value searching algorithm to determine first k, then by knowing k, $\lambda$.
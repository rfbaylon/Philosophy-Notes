# Modifying Summations
$\large\sum_{i=0}^n x^i = \large\sum_{i=1}^{n+1} x^{i-1}$

# Common Sums
## Geometric Sums
The most focus on in Discrete, used all the time in algorithms
$x \neq 1$
$\large\sum_{i=0}^n x^i = \frac{x^{n+1} - 1}{x-1}$

$\large\sum_{i=1}^n x^i = x\frac{x^{n} - 1}{x-1}$

$x = \frac{1}{2}$ no matter the $n$ is always approaching $2$
$x = 2$ no matter the $n$ is $2^{n+1} -1$

**Other Forms:**
$\large\sum_{i=0}^n x^i = \frac{x^{n+1} - 1}{x-1} = \frac{1-x^{n+1}}{1-x}$

$\large\sum_{i=0}^n a\cdot x^i = a \cdot \frac{x^{n+1} - 1}{x-1} = a \cdot \frac{1-x^{n+1}}{1-x}$

$\large\sum_{i=0}^{n-1} x^i = \large\sum_{i=1}^n x^{i-1} = \frac{x^n -1}{x-1} =  \frac{1- x^n}{1-x}$

Also, $\large\sum_{i=0}^\infty i\cdot x^i = \frac{x}{(1-x)^2}$

### Theta Notation
$\large\frac{x^{n+1} - 1}{x-1} =$

if $x>1$:  $\theta(x^n)$
if $x<1$: $\theta(1)$
either way, both are equal to $\theta$(largest term)

## Harmonic Sums

$\large\sum_{i=1}^n \frac{1}{i} = n$th harmonic number = ~$\ln n$
## Telescoping Sums

$\large\sum_{i=1}^n (F_{i} - F_{i-1}) = F_{n} - F_{0}$
## Arithmetic Sums

$\large\sum_{x=1}^n x = \frac{n(n+1)}{2}$


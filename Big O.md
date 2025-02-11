
#### Domination
A variable dominates when it is the term that creates the highest cieling or lowest floor (assuming that variable is gigantic)
Essentially *just* the term with the largest exponent. Logarithms and constants are simply just beat out in scale when you zoom out enough. 
- If variables are exponents, they are always the dominant term. 

Dominance Hierarchy:
- $n^n$
- $n!$
- $k^n$
- $n^k$
- $\log^k n$
- constants

# Big O
The ceiling.
If $f(n) \leq cn^3$ then $f(n) = O(n^3)$
Where there are terms in brackets, you find the Big O of each bracket and multiply them. For example, you could get a result like $O(n^.01 \cdot 3^n)$

# Omega
The floor.
If $f(n) \geq cn^3$ then $f(n) = \Omega(n^3)$

# Theta
If $f(n) =O(g(n))$ and $f(n) =\Omega(g(n))$ then $f(n) =\Theta(g(n))$

**Example**
![[Pasted image 20250210193207.png]]

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

### Big O
The ceiling.
If $f(n) \leq cn^3$ then $f(n) = O(n^3)$
Where there are terms in brackets, you find the Big O of each bracket and multiply them. For example, you could get a result like $O(n^.01 \cdot 3^n)$

- Any number occupies O(1) storage and can be read in O(1) time. Even irrationals.
- We can do simple arithmetic in O(1) time. 
- We care only about what happens at unimaginably large input sizes
- We focus on only worst-case time/space complexity.

Example:
**Prove $3n^2 + n + 2 = O(n^2)$**
This is equivalent to $3n^2 + n + 2 = Cn^2$ for $n \geq K$

### Omega
The floor.
If $f(n) \geq cn^3$ then $f(n) = \Omega(n^3)$

### Theta

If $f(n) =O(g(n))$ and $f(n) =\Omega(g(n))$ then $f(n) =\Theta(g(n))$
The constants and $n_1$ dont need to be the same between the O and Omega, but they could be. 

**Example**
![[Pasted image 20250210193207.png]]


## Proof by Exaggerate and Simplify

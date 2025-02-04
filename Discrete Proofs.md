
## Existence Proofs
Anything with the form $\exists x P(x)$
(there exists an x such that...)
### Constructive Proofs
Find a witness. If you can find one example of an x that satisfies $P(x)$, the proof has succeeded.

### Nonconstructive Proofs

#### Proof By Contradiction
Proofs that make use of the fact that $\lnot (p \land \lnot p)$
Helps to start by assuming the thing you are trying to prove is false and showing that it leads to a contradiction


#### Proof by Contraposition
Proofs that make use of the fact that $p \implies q$ is equivalent to $\lnot p \implies \lnot q$

#### Proof by Smallest Counterexample
Combines a proof by contradiction and a proof by induction.
The steps are as follows:
1. Create a base case where the theorem is true
2. If the theorem is incorrect, there exists a smallest counterexample ($k$).
3. Anything smaller than that counterexample ($k-1$) would not be a counterexample, and would generate a true statement
4. $k-1$ generates a false statement

##### Example
Theorem: For all $n\geqslant 1$, $\Large\sum\limits_{y=0}^n3^y < 3^{n+1}$
5. Base Case: $n=1$ is true. It equals 9.
6. If the theorem is false, there exists a smallest counter example. Call this counter example $k$. $\Large\sum\limits_{y=0}^k3^y < 3^{k+1}$
7. Since $k-1$ doesnt correspond to a counterexample, $\Large\sum\limits_{y=0}^{(k-1)}3^y < 3^{k}$
8. Add $3^k$ to both sides $\Large\sum\limits_{y=0}^k3^y < 3^k + 3^k$
9. Obtain a contradiction as $\Large 3 * 3^k < 2* 3^k$ is false

### Pigeonhole Principle
If k is a positive integer and k + 1 or more objects are placed into k boxes, then there is at least one box containing two or more of the objects.

![[Pasted image 20250203193459.png]]

Further, If N objects are placed into k boxes, then there is at least one box containing at least (N / k) objects.

**Example**: Among 100 people there are at least (100 / 12) = 9 who were born in the same month.
People are the pigeons, months are the holes.
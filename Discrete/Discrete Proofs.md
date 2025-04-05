---
Course: Discrete Mathematics
---
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

## Proof By Induction

If we tip the first domino, the nth domino falls as well.
If we tip the $k$ domino, the $k+1$ domino falls as well.
Likewise, if we tip the first domino (let $n$ be the last domino), $n-1$ falls. If $n-1$ falls, $n$ falls.

You want to prove something invoving $n$. There are 3 steps.
1. Assume that its true if you have $n-1$ (**Inductive Hypothesis**)
2. Prove that assumption 1 helps (**Inductive Step**)
3. Prove what you need for a small value (**Base Case)**

**Example:** Prove for all $n'  Fn \geq 1.7^n$
"For all fibonacci numbers greater than or equal to 2, prove the $n$th fibonacci number is $\leq 1.7^n$" 
1. Base cases: n=1 & n=2 are trivially true
2. Assume $F\small n-1$ $\leq 1.7^{n-1}$ and  $F\small n-2$ $\leq 1.7^{n-2}$

#### Weak and Strong Induction
[Good Video](https://www.youtube.com/watch?v=Ixtq64cUEHI)
**Statement of weak induction:** 
Let S(n) denote a statement regarding an integer n, and let k∈Z be fixed. 
If
- (i) S(k) holds, and
- (ii) for every m≥k,S(m)→S(m+1)

then for every n≥k, the statement S(n) holds.

**Statement of strong induction:** 
Let S(n) denote a statement regarding an integer n.
If
- (i) S(k) is true and
- (ii) for every m≥k,\[S(k)∧S(k+1)∧⋯∧S(m)]→S(m+1)

then for every n≥k, the statement S(n) is true.

#### Misc Notes
But be careful:
- not all proofs by induction require just one base case or one inductive step!
	- Sometimes claim $n$ relies on multiple smaller claims, and for each of those claims will need a base case.
	- You need one base case per inductive hypothesis
- You cant bridge the gap between $n$ and $n-1$  by using a finite example (eg 99-100)
- Sometimes you will see the inductive step assuming that claim $n$ is known and using it to prove $n+1$. This is the same as the above method, its a matter of style. 
- The base case is not always the smallest number.
	- Sometimes a claim is true only for larger values (eg $2^n > n^5$)
	- Sometimes $n$ just wont rely on the smallest instance
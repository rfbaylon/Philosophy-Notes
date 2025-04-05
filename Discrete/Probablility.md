
Sample Space: the amount of possible outcomes

problem: Roll 10 dice. Whats the probability there are no 1s?
answer: the sample space is $6^{10}$ and there are 5 ways for each dice to roll a ~1. So there are $5^{10}$ winning possibilities. Thus, $\frac{5^{10}}{6^{10}}$
Another way, is $\frac{5}{6}^{10}$. The 5/6 justified as those are the odds of winning on one die.

Note that when a problem asks "what are the odds at least one person does x...", its much easier to find the probability that that person doesnt do x.

what is the probability, in a group of $k$ people, that one is born on may 9th? 
answer: $1 - (\frac{364}{365})^k$

### Inclusion Exclusion

P(A $\lor$ B) = P(A) + P(B) - P(A $\land$ B)

Generalized here:
![[Pasted image 20250405092254.png]]
# Conditional Probability
| means 'given that,' and is completely different from $\cap$. What it does is reduce the sample space from $(B \cup \lnot B)$ to just B. So B effectively equals 1.

$P (A | B) = \frac{P(A \cup B)}{P(B)}$

When the unconditional and conditional probability are the same, event A is independent of event B. The chances of B dont at all impact the chances of A.

Example: what are the odds of the first of 3 coin flips being heads given that the third is heads?

base: 1/2
$P(A|B) = 

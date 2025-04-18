
![[Pasted image 20250402095649.png]]

1 Problem, 4 ways

- OR: how many ways could we make a committee of 3 different roles from 12 people where each person hold any number of roles?
	- 12^3
- O~R:How many ways could we make a committee of 3 different roles from 12 people where each person may only do one role?
	- $=\large{\frac{12!}{9!}}$
- ~O~R: How many ways could we form a committee of 3 people where all of the roles are shared from 12 people?
	- $=\large{\frac{12!}{9! \cdot 3!}}$
- ~OR: How many ways could we make a committee of 3 different roles with 12 different kinds of people?
	- $=\large{\frac{12+3-1}{(3-1)!}}$

## Ordered, Rep Allowed
h hats, t shirts, s shoes, j jeans
With one of each, there are $h * t * s * j$ ways to dress.

2 hats that can be worn on 7 days. $2^7$ ways to wear two hats.
n hats on 0 days = 1

Order matters means 001100 =/= 100100

How many binary numbres have length less than k?
Consider binary of lengths k, k-1, k-2
k=4: 1??? = 2^3
3: 1?? = 2^2
2: 1? = 2

### Problems

How many different license plate numbers with 3 letters followed by 3
numbers are possible?
Solution: $26^3 \cdot 10^3$

## Ordered, Rep Disallowed

$\large{\frac{n!}{(n-k)!}}$ = P(n,k)

### Problems
if you have 2 hats to wear across 7 days, but a different hat must be worn every day
This is equal to 7! / 5! (7 options first day, 6 the next, but there are no more days so it ends there)

if you have 7 hats to weat acaross 7 days, but you must wear a different hat every day.
  This is equal to 7! (7 options first day, 6 the next, 5 the next etc)

Its worth thinking about this as P(n,n) = $\large{\frac{n!}{(n-n)!} = \frac{n!}{1} = n!}$

## Unordered, Rep Allowed

$\large{\frac{n!}{(n-k)! \cdot k!}}$ = C(n,k)

## Unordered, Rep Unallowed

AKA Multichoose, Stars and Bars

K = Stars
N = Bars

 $\large{\frac{(k+n-1)!}{((k+n-1)-k)! \cdot k!} = \frac{(n-1 + k)!}{(n-1)! \cdot k!}}$ = C(k+n-1, k)


**Example**: The number of ways to select 5 fruits from 3 types of fruits (apples, bananas, oranges) where repetition is allowed is: $\large{C(3+5-1, 5)}$

$k = 5$
$n=3$

**So $k$ is the total fruits (stars) and $n$ is the number of types of fruits (bars)**

### Problems

You have 11 Biographies and 8 Mysteries that you want to arrange on your
bookshelf, but no two mysteries can be adjacent to each other. How many different
rearrangements are possible?
C(8+11+1-1, 11+1-1) = C(19,11) = 
(the +1 is because mysteries could be at front and back)

## Derangements
A derangement is an arrangement where each value in positoin cannot be repeated.
For example, from A, B, and C, the only derangements are ABC, CAB, and BCA.

Derangement formula:
$n!(1-\frac{1}{1!} + \frac{1}{2!} - ... + (-1)^n \frac{1}{n!}$

This converges to $e^{-1}$ as $n$ gets bigger, making the simpler formula for the amount of derangements: $\large{\frac{n!}{e}}$
Probability of a derangement: $\frac{1}{e}$


![[Pasted image 20250402095649.png]]

1 Problem, 4 ways

- OR: how many ways could we make a committee of 3 different roles from 12 people where each person hold any number of roles?
	- 12^3
- O~R:How many ways could we make a comittee of 3 different roles from 12 people where each person may only do one role?
	- $=\large{\frac{12!}{9!}}$
- ~O~R: How many ways could we form a committee of 3 people where all of the roles are shared from 12 people?
	- $=\large{\frac{12!}{9! \cdot 3!}}$

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


## Ordered, Rep Disallowed
  if you have 7 hats to weat acaross 7 days, but you must wear a different hat every day.
  This is equal to 7! (7 options first day, 6 the next, 5 the next etc)

Its worth thinking about this as P(n,n) = $\large{\frac{n!}{(n-n)!} = \frac{n!}{1} = n!}$

if you have 2 hats to wear across 7 days, but a different hat must be worn every day
This is equal to 7! / 5! (7 options first day, 6 the next, but there are no more days so it ends there)

$\large{\frac{n!}{(n-k)!}}$ = P(n,k)

## Unordered, Rep Allowed

$\large{\frac{n!}{(n-k)! \cdot k!}}$ = C(n,k)

## Unordered, Rep Unallowed

AKA Multichoose, Stars and Bars
 
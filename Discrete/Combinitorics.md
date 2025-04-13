
![[Pasted image 20250402095649.png]]

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

Its worth thinking about this as P(n,n) = $\frac{n!}{(n-n)!} = \frac

## Ordered, Rep Disallowed
  if you have 7 hats to weat acaross 7 days, but you must wear a different hat every day.
  This is equal to 7! (7 options first day, 6 the next, 5 the next etc)

if you have 2 hats to wear across 7 days, but a different hat must be worn every day
This is equal to 7! / 5! (7 options first day, 6 the next, but there are no more days so it ends there)

$\large{\frac{n!}{(n-k)!}}$ = P(n,k)

## Unordered, Rep Allowed


## Unordered, Rep Unallowed


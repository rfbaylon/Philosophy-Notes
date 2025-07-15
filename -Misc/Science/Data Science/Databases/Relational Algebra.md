---
Course: Database Design
---

A procedural query language for relations that allow us to retreive information from a relatoinal database.
- a quieryt is an operation applied to one or more relatoin instances
- RA is closed, meaning the result of a query is another relation
- Order of operaitons matters

8 basic operations
1. Select ($\sigma$)
2. Project ($\pi$)
	1. Returns a relation with a subset of attributes (select columns)
3. Rename ($\rho$)
	1. If youre renaming the relation, $\rho _{newname} {(oldname)}$
4. Cartesian Product ($\times$)
5. Join ($\Join$)
	1. A subset of the cartesian product
	2. Natural Join: ($\Join$)  join relations on attributes with the same name
	3. Theta Join ($\Join _{\Theta}$) Join relations with explicitly supplied join predicates
	4. The schema of the resulting relation is $attr(A) \cup attr(B)$
	5. If there are no common attributes, it returns the cartesian product
6. Intersection ($\cap$)
7. Set difference ($-$)
8. Union ($\cup$)
	1. Intersection, set difference, and union are the same as in [[Set Theory]], but the one difference is that relations must be **schema compatible**. That means they have the same kinds of attributes and the same number of attributes


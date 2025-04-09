---
Course: Discrete Mathematics
---

# Operators

### Operators

#### **And** $\land$

| P   | Q   | P and Q |
| --- | --- | ------- |
| T   | T   | T       |
| T   | F   | F       |
| F   | T   | F       |
| F   | F   | F       |
Communicative Property:
$(A \land B) \iff (B \land A)$

Associative Property
$(A \land B) \land C \iff A \land (B \land C)$

Identity Property
$A \iff A$

Idempotence Property
$A \land A \iff A$

#### Or
**Inclusive Or** $\lor$

| P   | Q   | P Or Q |
| --- | --- | ------ |
| T   | T   | T      |
| T   | F   | T      |
| F   | T   | T      |
| F   | F   | F      |

**Exclusive Or** $\oplus$

| P   | Q   | P XOR Q |
| --- | --- | ------- |
| T   | T   | F       |
| T   | F   | T       |
| F   | T   | T       |
| F   | F   | F       |

Distributivity between AND and OR
$A \land (B \lor C) \iff (A \land B) \lor (A \land C)$

DeMorgan's Laws
$\lnot(A \land B) \iff \lnot A \lor \lnot B$
$\lnot(A \lor B) \iff \lnot A \land \lnot B$

$A \land (B \lor C) \iff (A \land B) \lor (A \land C)$

#### CNF and DNF
**Conjunctive Normal Form** is what happens when $\land$ is outside of the parenthesis. 
For example: $A \land (B \lor C)$

**Disjunctive Normal Form** is what happens when $\lor$ is outside of the parenthesis.
For example: $(A \land B) \lor (A \land C)$

Any propositional formula can be written in either CNF or DNF. 

## Implication

**Implies** $\implies$

| P   | Q   | P If Q |
| --- | --- | ------ |
| T   | T   | T      |
| T   | F   | F      |
| F   | T   | T      |
| F   | F   | T      |

**If and Only If** $\iff$

| P   | Q   | P Iff Q |
| --- | --- | ------- |
| T   | T   | T       |
| T   | F   | F       |
| F   | T   | F       |
| F   | F   | T       |

# Valid Formulas

1. $P \lor \lnot P$

# For All / There Exists

$\forall$ For All
$\exists$ There Exists

These two sentences mean the same thing:
- There is no one who likes being mocked
- Everyone dislikes being mocked.

This means that:
$\lnot (\forall x. P(x)) \iff \exists x. \lnot(P(x)).$
	The general principle is that moving a NOT to the other side of an “$\exists$” changes it into “$\forall$,” and vice versa.



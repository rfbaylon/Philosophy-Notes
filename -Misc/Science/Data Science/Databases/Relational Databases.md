---
Course: Database Design
---


Table Name = Relation
Rows = Tuples
Columns = Attributes



The relational model provides a formal mathematical basis for the structure of and interaction with a relational database. Its based on [[Set Theory]] and first order predicate logic

Good Design
- Say NO to composite attributes (ex address that includes city, state, zip, etc)
- Say NO to multivaried attributes (all email addresses for one person)

## Keys
The primary key is the attribute that cannot be null and serve as the reference to compare each tuple.

The super key of a relation is any set of tuple that is unique. For example, there is only one instance of an ID, so it (and any combination of an ID and other attribute) is a super key

A foreign key (FK) is the key I use to to translate one data table to another. A foreign key is also the Referential Integrety Constraint
### Tuple
Like a list, but immutable
tuple = ()
	(1, 2, 3)

with a tuple, we **can** create, index, iterate by value, or iterate by position
Its different from a list because in a tuple, we cannot append, remove, or modify in any way.

Why use tuples?
- Protect data from being modified
- More memory effecient than a list
- Pretend to return 2 things from a function
	def test():
		code, 
		code,
		code,
		return: x, y
	This code returns just ONE thing, but as a tuple. 

### Sets
Just like the math theory
set = {}

- Unordered (no index)
	{1, 2, 3} = {2, 1, 3}
- No duplicates
	{1, 1, 1, 2, 2, 3} = {1, 2, 3}
- Mutable BUT elements are immutable

We can...
- Create a set
- Set of ints, strings, tuples, or floats
- add to set 
	set.add()
- remove from a set
	set.remove()
- iterate by value

We cant...
- Create a set of lists, sets, or dictionaries
- index a set
- sort
- iterate by position (for or while loop)

Why use sets?
- answering "is this thing in this set?" effeciently
- deduping*
	if you turn a list into a set, there are no more duplicates
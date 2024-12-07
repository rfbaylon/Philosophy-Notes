Numpy makes arrays
	Uses [] like lists do, but it computes much faster than python lists
	VERY good choice for data sets with lots of numeric data
Friends with [[Pandas]] :)

# Basics
ray = np.array([4, 5, 6])
	creates a 1d array that acts like a python list
z = np.zeros((3,))
	creates an array full of zeros
	returns [0,0,0]
ray.shape
	returns (3,)

ray2d = np.array ([[4, 5, 6], [7,8,9]])
	creates 2d array
ray2d.shape
	returns (2, 3)
ray2d.reshape(3,2)
	returns [[4, 5],[6, 7],[8, 9]]

np.where(condition, if true, if false)
	used a lot with [[Pandas]]
np.where(ray %2 == 0, "even", "odd")
	returns ["even", "odd", even"]

np.fromfunction(lambda i, j: i * 20 + j, (3, 1)
	creates array based on a function (often a lambda)
	returns: [[0], [20], [40]]
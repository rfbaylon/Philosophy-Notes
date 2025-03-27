
## Merge Sort
T(n) Time function, $n$ is the amount of elements

Merging one array:
**Takes $2\cdot T(\frac{n}{2}) + \Theta(n)$ Time** 
1. Start by dividing the problem into smaller parts
2. Then conquer (solve) the smaller problems
	1. Note: You can even further mergesort the smaller problems
3. Then merge the solutions
4. Then solve the merged solutions

- Divide take $\Theta(1)$ time
- Conquer takes $\Theta(1) + 2 \cdot T(\frac{n}{2})$ time
- Merge takes $\Theta(n)$ time


Merging 2 sorted arrays:
**Takes $\Theta(n)$ time**
5. Compare index 1 in array A and Array B
6. If index 1 in A is smaller, copy that value to the output array
7. Add one index position to A and repeat (so youd compare index 2 in A and index 1 in B).


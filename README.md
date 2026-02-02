**In NumPy, dimensions = number of axes.**

Object	Example	ndim	Why
Scalar	25	0	No axes (Single point)
1D array	[1, 2, 3]	               1  One axis (length)
2D array	[[1, 2], [3, 4]]	       2	Rows + columns
3D array	Stack of matrices	       3	Depth + rows + columns


**A quick intuition**

Think of dimensions like directions you can move:

0D → nowhere to move (just a point)

1D → left/right

2D → left/right, up/down

3D → left/right, up/down, in/out



print(type(n))
print(n.dtype)
print(n.ndim)



**1. type(n)
<class 'numpy.ndarray'>


This shows that n is an instance of NumPy’s ndarray class.

ndarray stands for N-dimensional array.

Unlike Python lists, NumPy arrays:

Store elements of the same data type

Are optimized for fast numerical computation

Support vectorized operations

✅ This confirms that n is a NumPy array, not a Python list.

2. n.dtype
float64


dtype (data type) describes the type of elements stored in the array.

float64 means:

Each element is a 64-bit floating-point number

This is NumPy’s default numeric type

Even though we created the array using zeros, NumPy uses floating-point values (0.0) unless a different type is specified.

You can change the data type like this:

n = np.zeros((4, 4), dtype=int)

3. n.ndim
2


ndim stands for number of dimensions

It tells you how many axes the array has

For this array:

Axis 0 → rows

Axis 1 → columns

Because it has two axes, n is a 2-dimensional array.**

# NumPy Cheatsheet

NumPy is a popular Python library for numerical computing. It provides a wide range of tools for working with arrays, matrices, and numerical operations. This cheatsheet provides a quick reference for some of NumPy's unique features, including code blocks for creating arrays, indexing, slicing, broadcasting, and more. Additionally, it includes a list of resources for further learning.

## Creating Arrays

```python
import numpy as np

# Create a 1D array
x = np.array([1, 2, 3])

# Create a 2D array
y = np.array([[1, 2], [3, 4]])

# Create an array of zeros
np.zeros((3, 3))

# Create an array of ones
np.ones((2, 2))

# Create an array with a range of values
np.arange(0, 10, 2)

# Create an array with random values
np.random.rand(3, 3)

# Create an array with normally distributed random values
np.random.randn(3, 3)
```

## Indexing and Slicing

```python
# Index a 1D array
x[0]

# Index a 2D array
y[0, 1]

# Slice a 1D array
x[1:3]

# Slice a 2D array
y[:, 1]

# Boolean indexing
x[x > 2]
```

## Broadcasting

```python
# Add a scalar to an array
x + 1

# Add two arrays
x + y

# Multiply two arrays
x * y

# Multiply an array by a scalar
x * 2
```

## Other Useful Features

```python
# Compute the dot product of two arrays
np.dot(x, y)

# Transpose an array
y.T

# Reshape an array
x.reshape((3, 1))

# Compute the sum of an array
x.sum()

# Compute the mean of an array
x.mean()

# Compute the standard deviation of an array
x.std()
```

## Resources

- [NumPy documentation](https://numpy.org/doc/stable/)
- [NumPy quickstart tutorial](https://numpy.org/doc/stable/user/quickstart.html)
- [Python Data Science Handbook](https://jakevdp.github.io/PythonDataScienceHandbook/index.html)
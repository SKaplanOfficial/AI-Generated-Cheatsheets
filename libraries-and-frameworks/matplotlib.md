# Matplotlib Cheatsheet

Matplotlib is a popular plotting library for Python. It provides a wide range of tools for creating static, animated, and interactive visualizations in Python. This cheatsheet provides a quick reference for some of Matplotlib's unique features, including code blocks for basic plots, subplots, customization, and more. Additionally, it includes a list of resources for further learning.

## Basic Plots

```python
import matplotlib.pyplot as plt
import numpy as np

# Create a simple line plot
x = np.linspace(0, 10, 100)
y = np.sin(x)
plt.plot(x, y)
plt.show()

# Create a scatter plot
x = np.random.rand(100)
y = np.random.rand(100)
plt.scatter(x, y)
plt.show()

# Create a histogram
x = np.random.normal(size=1000)
plt.hist(x, bins=30)
plt.show()
```

## Subplots

```python
# Create a figure with multiple subplots
fig, axs = plt.subplots(2, 2, figsize=(6, 6))
axs[0, 0].plot(x, y)
axs[0, 1].scatter(x, y)
axs[1, 0].hist(x, bins=30)
axs[1, 1].imshow(np.random.rand(100, 100))
plt.show()
```

## Customization

```python
# Add a title and axis labels
plt.plot(x, y)
plt.title('Sine Wave')
plt.xlabel('X')
plt.ylabel('Y')
plt.show()

# Customize the style
plt.style.use('ggplot')
plt.plot(x, y)
plt.show()

# Add a legend
plt.plot(x, np.sin(x), label='sin(x)')
plt.plot(x, np.cos(x), label='cos(x)')
plt.legend()
plt.show()
```

## Other Useful Features

```python
# Save a figure to a file
plt.plot(x, y)
plt.savefig('figure.png')

# Clear the current figure
plt.clf()

# Close all figures
plt.close('all')
```

## Resources

- [Matplotlib documentation](https://matplotlib.org/stable/contents.html)
- [Matplotlib tutorials](https://matplotlib.org/stable/tutorials/index.html)
- [Python Data Science Handbook](https://jakevdp.github.io/PythonDataScienceHandbook/index.html)
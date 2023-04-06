# Wolfram Language Cheatsheet

Wolfram Language is a general-purpose programming language developed by Wolfram Research. It is particularly well-suited for symbolic computation and data analysis. Here is an overview of some of its basic syntax and features.

## Basic Operations

### Arithmetic
```
2 + 2
3 * 4
5 / 2
```

### Variables
```
x = 42
y = 3.14
z = "hello"
```

### Lists
```
list = {1, 2, 3, 4, 5}
list[[3]]
```

### Functions
```
f[x_] := x^2
f[3]
```

## Data Analysis

### Importing Data
```
data = Import["filename.csv"]
```

### Manipulating Data
```
Mean[data]
Median[data]
StandardDeviation[data]
```

### Plotting Data
```
ListPlot[data]
Histogram[data]
```

## Symbolic Computation

### Algebra
```
Expand[(x + y)^3]
Factor[x^3 - y^3]
Solve[x^2 + y^2 == 1, y]
```

### Calculus
```
D[x^2, x]
Integrate[x^2, x]
```

### Differential Equations
```
DSolve[y'[x] == y[x], y[x], x]
```

## Resources

- [Wolfram Language Documentation](https://www.wolfram.com/language/)
- [Wolfram Language Tutorial Collection](https://www.wolfram.com/language/elementary-introduction/)
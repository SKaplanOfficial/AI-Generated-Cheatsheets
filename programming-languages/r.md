## R Cheatsheet

### Overview

R is a programming language and environment for statistical computing and graphics. It is widely used in data analysis, machine learning, and scientific research. R was created by Ross Ihaka and Robert Gentleman at the University of Auckland, New Zealand in 1993.

### Variables

R variables can store a variety of data types, including numeric, character, logical, and complex. Variables are assigned using the `<-` or `=` operator.

```r
# Numeric variable
x <- 3.14

# Character variable
name <- "Alice"

# Logical variable
is_female <- TRUE

# Complex variable
z <- 1 + 2i
```

### Functions

R has a large number of built-in functions for common tasks such as data manipulation, statistical analysis, and plotting. Functions are called by name, with arguments in parentheses.

```r
# Data manipulation
mean(c(1, 2, 3, 4, 5))  # Returns 3

# Statistical analysis
t.test(c(1, 2, 3, 4, 5), mu=3)  # One-sample t-test

# Plotting
plot(c(1, 2, 3, 4, 5), c(1, 4, 9, 16, 25), type="l")
```

### Loops

R has several types of loops, including `for`, `while`, and `repeat`. The `for` loop is used to iterate over a sequence of values, while the `while` and `repeat` loops are used to repeat a block of code while a condition is true or false.

```r
# For loop
for (i in 1:10) {
    print(i)
}

# While loop
i <- 1
while (i <= 10) {
    print(i)
    i <- i + 1
}

# Repeat loop
i <- 1
repeat {
    print(i)
    i <- i + 1
    if (i > 10) {
        break
    }
}
```

### Conditionals

R has several conditional statements, including `if`, `else if`, and `else`. These statements are used to control the flow of a program based on certain conditions.

```r
# If statement
age <- 30
if (age >= 18) {
    print("You are an adult")
}

# If-else statement
age <- 15
if (age >= 18) {
    print("You are an adult")
} else {
    print("You are a minor")
}

# If-else if-else statement
age <- 25
if (age < 18) {
    print("You are a minor")
} else if (age < 65) {
    print("You are an adult")
} else {
    print("You are a senior")
}
```

### File Manipulation

R provides several functions for manipulating files, including `read.csv`, `write.csv`, `file.rename`, and `file.remove`.

```r
# Read CSV file
data <- read.csv("data.csv")

# Write CSV file
write.csv(data, "data_new.csv")

# Rename file
file.rename("data.csv", "data_old.csv")

# Remove file
file.remove("data_old.csv")
```

### Resources

- [R documentation](https://www.r-project.org/documentation/)
- [RStudio](https://www.rstudio.com/) (integrated development environment)
- [CRAN](https://cran.r-project.org/) (community repository)
- [R for Data Science](https://r4ds.had.co.nz/) (online book)
# Fortran Cheatsheet

## Overview of unique features

- High-performance programming language
- Designed for scientific and engineering applications
- Supports array operations and linear algebra
- Uses verbose syntax
- Can be used for numerical simulations and modeling

## Variables

```fortran
PROGRAM MYPROGRAM
  IMPLICIT NONE
  INTEGER :: X = 42
  REAL :: Y
  PARAMETER (MYCONST = 10)
  INTEGER, DIMENSION(3) :: MYARRAY = [1, 2, 3]
END PROGRAM MYPROGRAM
```

## Functions

```fortran
FUNCTION ADD(X, Y)
  IMPLICIT NONE
  INTEGER, INTENT(IN) :: X, Y
  ADD = X + Y
END FUNCTION ADD

PROGRAM MYPROGRAM
  IMPLICIT NONE
  INTEGER :: RESULT
  RESULT = ADD(3, 4)
END PROGRAM MYPROGRAM
```

## Loops

```fortran
DO I = 1, 10
  ! do something
END DO

DO WHILE (CONDITION)
  ! do something
END DO
```

## Conditionals

```fortran
IF (X > Y) THEN
  ! do something
ELSE
  ! do something else
END IF
```

## Array operations

```fortran
REAL, DIMENSION(3) :: X = [1.0, 2.0, 3.0]
REAL, DIMENSION(3) :: Y = [4.0, 5.0, 6.0]

! Element-wise addition
X = X + Y

! Element-wise multiplication
X = X * Y

! Dot product
DOT_PRODUCT = DOT_PRODUCT(X, Y)
```

## Resources

- [Fortran documentation](https://fortran-lang.org/learn/)
- [Fortran tutorial](https://www.tutorialspoint.com/fortran/index.htm)
- [Fortran forum](https://stackoverflow.com/questions/tagged/fortran) for community support and troubleshooting.
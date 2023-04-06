# COBOL Cheatsheet

## Overview of unique features

- Business-oriented programming language
- Designed for handling large amounts of data
- Uses verbose syntax
- Supports file handling and database access
- Can be used for financial and administrative applications

## Variables

```cobol
IDENTIFICATION DIVISION.
PROGRAM-ID. MYPROGRAM.

DATA DIVISION.
WORKING-STORAGE SECTION.
01 MY-VARIABLE PIC 9(4).
01 MY-CONSTANT PIC X(10) VALUE "HELLO".
01 MY-ARRAY OCCURS 10 TIMES PIC 9(3).

PROCEDURE DIVISION.
```

## Functions

COBOL does not have functions in the same sense as high-level programming languages. Instead, it uses subroutines to perform specific tasks.

```cobol
IDENTIFICATION DIVISION.
PROGRAM-ID. MYPROGRAM.

DATA DIVISION.
WORKING-STORAGE SECTION.
01 MY-VARIABLE PIC 9(4).

PROCEDURE DIVISION.
  PERFORM MY-SUBROUTINE.

MY-SUBROUTINE.
  ADD 1 TO MY-VARIABLE.
```

## Loops

```cobol
IDENTIFICATION DIVISION.
PROGRAM-ID. MYPROGRAM.

DATA DIVISION.
WORKING-STORAGE SECTION.
01 I PIC 9(2).

PROCEDURE DIVISION.
  PERFORM VARYING I FROM 1 BY 1 UNTIL I > 10
    DISPLAY I
  END-PERFORM.
```

## Conditionals

```cobol
IDENTIFICATION DIVISION.
PROGRAM-ID. MYPROGRAM.

DATA DIVISION.
WORKING-STORAGE SECTION.
01 X PIC 9(3) VALUE 100.
01 Y PIC 9(3) VALUE 200.

PROCEDURE DIVISION.
  IF X > Y
    DISPLAY "X IS GREATER THAN Y"
  ELSE
    DISPLAY "Y IS GREATER THAN X"
  END-IF.
```

## File handling

```cobol
IDENTIFICATION DIVISION.
PROGRAM-ID. MYPROGRAM.

DATA DIVISION.
FILE SECTION.
01 MY-FILE.
  05 MY-NAME PIC X(10).
  05 MY-AGE PIC 9(3).

PROCEDURE DIVISION.
  OPEN INPUT MY-FILE.
  READ MY-FILE INTO MY-RECORD.
  CLOSE MY-FILE.
```

## Resources

- [COBOL documentation](https://www.ibm.com/docs/en/cobol/)
- [COBOL tutorial](https://www.tutorialspoint.com/cobol/index.htm)
- [COBOL forum](https://stackoverflow.com/questions/tagged/cobol) for community support and troubleshooting.
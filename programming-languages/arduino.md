# Arduino Cheatsheet

## Overview of unique features

- Microcontroller platform
- Simplified C++ programming language
- Integrated development environment (IDE)
- Built-in functions for interacting with hardware
- Wide range of compatible sensors and modules
- Real-time processing capabilities

## Variables

```C++
// Declare a variable
int x = 42;

// Declare a constant
const int y = 10;

// Declare an array
int myArray[3] = {1, 2, 3};

// Declare a string
String myString = "hello";
```

## Functions

```C++
// Declare a function
int add(int x, int y) {
  return x + y;
}

// Call a function
int result = add(3, 4);
```

## Loops

```C++
// Define a for loop
for (int i = 0; i < 10; i++) {
  // do something
}

// Define a while loop
while (condition) {
  // do something
}
```

## Conditionals

```C++
// Define an if-else statement
int max(int x, int y) {
  if (x > y) {
    return x;
  } else {
    return y;
  }
}
```

## Interacting with hardware

```C++
// Set up a digital pin
int ledPin = 13;
void setup() {
  pinMode(ledPin, OUTPUT);
}

// Turn on and off the LED
void loop() {
  digitalWrite(ledPin, HIGH);
  delay(1000);
  digitalWrite(ledPin, LOW);
  delay(1000);
}
```

## Resources

- [Arduino documentation](https://www.arduino.cc/reference/en/)
- [Arduino programming language tutorial](https://www.arduino.cc/en/Tutorial/Foundations)
- [Arduino forum](https://forum.arduino.cc/) for community support and troubleshooting.
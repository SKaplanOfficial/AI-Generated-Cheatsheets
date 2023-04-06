# Processing Cheatsheet

Processing is a programming language and development environment designed for creating visual and interactive applications. Here is an overview of its features, code blocks, and resources.

## Features

-    Processing is designed for creating visual and interactive applications, such as generative art, data visualization, and games.
-    It is based on Java and can be used for both desktop and web applications.
-    Processing provides a simplified syntax and a library of functions for working with graphics, sound, and input.
-    Processing is open source and has a large community of users and contributors.

## Code Blocks

### Setup and Draw

Processing programs are organized into two main code blocks: `setup()` and `draw()`. `setup()` is called once at the beginning of the program, and `draw()` is called repeatedly to update the display.

```java
void setup() {
    // code to be executed once at the beginning of the program
}

void draw() {
    // code to be executed repeatedly to update the display
}
```

### Variables

Variables are used to store data that can be used later in the program.

```java
int variableName = value;
```

### Functions

Functions are code blocks that perform a specific task. They can be called by other parts of the program.

```java
void functionName(parameter1, parameter2) {
    // code to be executed
}
```

### Conditionals

Conditionals allow the program to make decisions based on certain conditions.

```java
if (condition) {
    // code to be executed if condition is true
} else if (otherCondition) {
    // code to be executed if otherCondition is true
} else {
    // code to be executed if neither condition is true
}
```

### Loops

Loops allow the program to repeat a set of instructions.

```java
for (int i = 0; i < 10; i++) {
    // code to be executed
}
```

### Objects

Objects are a fundamental part of Processing and are used to store and manipulate data.

```java
class ClassName {
    int property1;
    float property2;

    ClassName(int p1, float p2) {
    property1 = p1;
    property2 = p2;
    }

    void method() {
    // code to be executed
    }
}

ClassName objectName = new ClassName(1, 2.0);
```

### Graphics

Processing provides a library of functions for working with graphics, including drawing shapes, colors, and images.

```java
// set the background color
background(255, 255, 255);

// draw a rectangle
rect(x, y, width, height);

// draw an ellipse
ellipse(x, y, width, height);

// load an image
PImage img = loadImage("image.png");

// display an image
image(img, x, y);
```

## Resources

Here are some resources for learning and using Processing:

- [Processing Documentation](https://processing.org/reference/)
- [Processing subreddit](https://www.reddit.com/r/processing/)
- [Processing Tutorial](https://processing.org/tutorials/)
- [Processing on Stack Overflow](https://stackoverflow.com/questions/tagged/processing)
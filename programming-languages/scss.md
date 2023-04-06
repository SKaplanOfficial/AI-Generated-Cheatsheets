# SCSS Cheatsheet

## Unique Features

- Sassy CSS, an extension of CSS
- Adds features like variables, nesting, and mixins
- Compiles to standard CSS syntax
- Allows for more efficient and organized stylesheet development

## Basic Syntax

```scss
$variable: value;

selector {
  property: $variable;
}
```

## Variables

```scss
$primary-color: #ff0000;

.selector {
  color: $primary-color;
}
```

## Nesting

```scss
.selector {
  font-size: 16px;

  .nested-selector {
    font-size: 12px;
  }
}
```

## Mixins

```scss
@mixin border-radius($radius) {
  -webkit-border-radius: $radius;
  -moz-border-radius: $radius;
  border-radius: $radius;
}

.selector {
  @include border-radius(5px);
}
```

## Operators

- `+`: Addition
- `-`: Subtraction
- `*`: Multiplication
- `/`: Division
- `%`: Modulus

## Control Directives

- `@if`: Conditional statement
- `@for`: Looping statement
- `@each`: Looping statement for lists
- `@while`: Looping statement

## Resources

- [Official SCSS Documentation](https://sass-lang.com/documentation)
- [Scotch.io SCSS Tutorial](https://scotch.io/tutorials/getting-started-with-sass)
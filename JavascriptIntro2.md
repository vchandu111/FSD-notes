## Relational operators

[TOC]

These operators allow you to test the relation between 2 values and returns a `boolean`. JavaScript unlike other languages allows you to compare any type with any other type!

### Greater than and greater than equal to

The **greater than** operator `>` allows you to check if one value is greater than the other. It returns `true` if the first value is greater than the second and `false` if the second value is greater.

```javascript
20 > 10 //true
10 > 20 //false
10 > 10 //false
10 >= 10 //true

```

### Lesser than and lesser than equal to

The **lesser than** operator `>` allows you to check if one value is lesser than the other. It returns `false` if the first value is greater than the second and `true` if the second value is greater.

```javascript
20 < 10 //false
10 < 20 //true
10 < 10 //false
10 <= 10 //true
```

## Conditional Statements



In JavaScript we have the following conditional statements:

- Use `if` to specify a block of code to be executed, if a specified condition is true
- Use `else` to specify a block of code to be executed, if the same condition is false
- Use `else if` to specify a new condition to test, if the first condition is false
- Use `switch` to specify many alternative blocks of code to be executed

## The if Statement

Use the `if` statement to specify a block of JavaScript code to be executed if a condition is true.

Example: Make a "Good day" greeting if the hour is less than 18:00:

```javascript
if (hour < 18) {
  greeting = "Good day";
}
output:Good day
```

## The else Statement

Use the `else` statement to specify a block of code to be executed if the condition is false.

```javascript
if (condition) {
  //  block of code to be executed if the condition is true
} else {
  //  block of code to be executed if the condition is false
}
```

Example : If the hour is less than 18, create a "Good day" greeting, otherwise "Good evening":

```javascript
if (hour < 18) {
  greeting = "Good day";
} else {
  greeting = "Good evening";
}
```

## The else if Statement

Use the `else if` statement to specify a new condition if the first condition is false.

```javascript
if (condition1) {
  //  block of code to be executed if condition1 is true
} else if (condition2) {
  //  block of code to be executed if the condition1 is false and condition2 is true
} else {
  //  block of code to be executed if the condition1 is false and condition2 is false
}
```

Example : If time is less than 10:00, create a "Good morning" greeting, if not, but time is less than 20:00, create a "Good day" greeting, otherwise a "Good evening":

```javascript
if (time < 10) {
  greeting = "Good morning";
} else if (time < 20) {
  greeting = "Good day";
} else {
  greeting = "Good evening";
}
```

## Ternary operator

### Syntax:

```
condition ? true : false
```

## Switch Statement

The `switch` statement is used to perform different actions based on different conditions.

### Syntax:

```javascript
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
```

This is how it works:

- The switch expression is evaluated once.
- The value of the expression is compared with the values of each case.
- If there is a match, the associated block of code is executed.
- If there is no match, the default code block is executed.

**Example:**

```javascript
var day = 6
switch (day) {
  case 0:
    day = "Sunday";
    break;
  case 1:
    day = "Monday";
    break;
  case 2:
    day = "Tuesday";
    break;
  case 3:
    day = "Wednesday";
    break;
  case 4:
    day = "Thursday";
    break;
  case 5:
    day = "Friday";
    break;
  case 6:
    day = "Saturday";
    break;
  default:
    day = "Invalid Input";
}
console.log(day)
```


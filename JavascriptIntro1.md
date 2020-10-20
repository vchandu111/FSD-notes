# JavaScript:

- [JavaScript](https://developer.mozilla.org/en-US/docs/Glossary/JavaScript) is a scripting language that enables you to create dynamically updating content, control multimedia, animate images, and pretty much everything else. (Okay, not everything, but it is amazing what you can achieve with a few lines of JavaScript code.)

  

  [TOC]

  

### Variables:

**Variables** in JavaScript are used to store different kinds of data. Think of a variable like a bottle. We use bottles to store water, in much the same way we use variables to store various forms of data in JavaScript.

*example*: 

```javascript
var x = 200
```

You can also declare multiple variables in one statement as seen in the syntax above.

*example*: 

```javascript
var a = 100, b = 200, c = 300
```

```javascript
var x = 5; 	//x stores the value 5
var y = 6	//y stores the value 6
var z = x + y //z  stores value of 5+6 =11


```



## Data Types In JavaScript:

There are 7 ***primitive*** types of data in JavaScript

```javascript
var length = 16;                               // Number
var lastName = "Johnson";                      // String
var x = {firstName:"John", lastName:"Doe"};    // Object
```

```javascript
var x = 16 + "Volvo" and 
var x = "16" + "Volvo" 
When adding a number and a string, JavaScript will treat the number as a string.
Output for above code is 16Volvo


```

```javascript
var x = 16 + 4 + "Volvo"  //output:20Volvo
var x = "Volvo" + 16 + 4  //output:Volvo164
In the first example, JavaScript treats 16 and 4 as numbers, until it reaches "Volvo".

In the second example, since the first operand is a string, all operands are treated as strings.
```

### Strings:

The first type of data is a `String`. This is used to store a sequence of characters used to represent text.

```javascript
var name = "Masai School"  
```

Any data within quotes `" "` is a String in JavaScript.

### Numbers:

The second type of data we want to know is a `Number`, which is used to store any kind of numbers.

```javascript
var num = 100
var dec = 100.001
```

### Booleans:

You can use the `Boolean()` function to find out if an expression (or a variable) is true:

```javascript
var x = 5;
var y = 5;
var z = 6;
(x == y)       // Returns true
(x == z)       // Returns false
```

Booleans are often used in conditional testing.



```javascript
var x = 0;
Boolean(x);       // returns false

var x = -0;
Boolean(x);       // returns false

var x = "";
Boolean(x);       // returns false

var x;
Boolean(x);       // returns false

var x = null;
Boolean(x);       // returns false

var x = false;
Boolean(x);       // returns false

var x = 10 / "H";
Boolean(x);       // returns false
```



## JavaScript Arrays:

JavaScript arrays are written with square brackets.

Array items are separated by commas.

```javascript
var cars = ["Saab", "Volvo", "BMW"];
```

Array indexes are **zero-based**, which means the first item is [0], second is [1], and so on.

## The typeof Operator

You can use the JavaScript `typeof` operator to find the type of a JavaScript variable.

The `typeof` operator returns the type of a variable or an expression:

```javascript
typeof ""             // Returns "string"
typeof "John"         // Returns "string"
typeof "John Doe"     // Returns "string"
typeof 0              // Returns "number"
typeof 314            // Returns "number"
typeof 3.14           // Returns "number"

var name = "Masai School"
console.log(typeof(name)) //returns string
```

## Mathematical operators in JavaScript

| Operator |  Description   |
| :------: | :------------: |
|    +     |    addition    |
|    -     |  subtraction   |
|    *     | multiplication |
|    **    | exponentiation |
|    /     |    division    |
|    %     |    modulus     |
|    ++    |   increment    |
|    --    |   decrement    |
|          |                |

```javascript
var a = 2
var b = 3
var c = a + b
var d = a * b
var e = a / b 
var f = a - b

Output :
c = 5
d = 6
e = 0.6666666666666666
f = -1
```

### Modulo or Remainder Operator:

Many programming languages including JavaScript have a modulo operator `%`. This operator returns the remainder when one variable is divided by another.

- ```javascript
  var x = 5;
  var y = 2;
  var z = x % y;
  Output: 1
  ```

- ```javascript
  var a = 10 % 2
  var b = 11 % 2
  output :
  a = 0
  b = 1
  ```

## Exponentiation:

The **exponentiation** operator (`**`) raises the first operand to the power of the second operand.

```javascript
var x = 5;
var z = x ** 2 = 5**2        // result is 25
```

x ** y produces the same result as `Math.pow(x,y)`:

## Increment and Decrement Operator:

In programming we often want to increment or decrement an operator by just one value. For example we have a variable `age = 20` which increases every year. For this we use the `++` operator also called **increment operator** to increase the value of `age` by 1.

```javascript
var birthday = 20
birthday++  //returns 21
```

### Postfix increment:

If used postfix, with operator after operand (for example, `x++`), the increment operator increments and returns the value before incrementing.

```javascript
let x = 3;
y = x++
console.log(y) //returns 3
console.log(x) //returns 4
```

### Prefix increment:

If used prefix, with operator before operand (for example, `++x`), the increment operator increments and returns the value after incrementing.

```javascript
let x = 3;
y = ++x
console.log(y) //returns 4
console.log(x) //returns 4
```

### Postfix decrement:

If used postfix, with operator after operand (for example, `x++`), the increment operator increments and returns the value before incrementing.

```javascript
let x = 3;
y = x--
console.log(y) //returns 3
console.log(x) //returns 2
```

### Prefix decrement:

If used prefix, with operator before operand (for example, `++x`), the increment operator increments and returns the value after incrementing.

```javascript
let x = 3;
y = --x
console.log(y) //returns 2
console.log(x) //returns 2
```



| *Operator* | ***Example*** | *Same As*  |
| :--------: | :-----------: | :--------: |
|     =      |     x = y     |   x = y    |
|     +=     |    x += y     | x = x + y  |
|     -=     |    x -= y     | x = x - y  |
|     *=     |    x *= y     | x = x * y  |
|     /=     |    x /= y     | x = x / y  |
|     %=     |    x %= y     | x = x % y  |
|    **=     |    x **= y    | x = x ** y |



## String concatenation:

A special property of `Strings` is that they can be combined or concatenated with one another.

```javascript
var word1 = "Welcome"
var word2 = "Masai"
var word3 = word1 + " to " + word2 + " school!"
console.log(word3) 
output : Welcome to Masai school!
```



## Converting between types:



Often we may have data in one type for example `string` and we may want to convert into another type for example `number` in order to do some calculations or to simply display the number.

To convert from a `string` to a `number` we can use the `Number()` function.



```javascript
var num1 = "12"
var num2 = "13"
console.log(num1 + num2)
Output: 1213


num1 = Number(num1)
num2 = Number(num2)
console.log(num1 + num2)
Output: 25
```



On the other hand to convert a `number` to a `string` we can use the `.toString()` function.

```javascript
Example 1:
var num1 = 12
var num2 = 13
console.log(num1 + num2)
output: 25
Example 2:
num1 = num1.toString()
num2 = num2.toString()
console.log(num1 + num2)
output:1213
```

## Comparison Operators

### Equality

The **equality** operator `==` lets you test if two values are equal or not. It accepts 2 inputs of any type and outputs `true` if they are equal and `false` if the are not equal.

```javascript
1 == 1  //true
1 == 2	//false
"Masai" == "Masai" //true
"Masai" == "masai" //false
```

### Inequality Operators:

The **inequality** operator `!=` performs the opposite function of the equality operator. It accepts 2 inputs of any type and outputs `false` if they are equal and `true` if the are not equal.



```javascript
1 != 1 //false
1 != 2 //true
"Masai" != "Masai" //false
"Masai" != "masai" //true

1 != '1' // false
1 !== '1' // true
```

| Operator |                 Description                  |
| :------: | :------------------------------------------: |
|    ==    |       equal to (checks only for value)       |
|   ===    | Strict Equal to (checks both value and type) |
|    !=    |                 not equal to                 |
|   !==    |      not equal value or not equal type       |
|    >     |                 greater than                 |
|    <     |                  less than                   |
|    >=    |           greater than or equal to           |
|    <=    |            less than or equal to             |
|    ?     |               ternary operator               |



## Logical operators

### AND, OR and NOT Operators

Logical operators are usually used with `Boolean` values as inputs. The outputs are also `Boolean` values.

**AND Operator**

Lets say you want to check if 2 conditions in your program are true. The `&&` operator compares 2 `boolean` values and returns `true` when both `boolean` values are `true`.

```javascript
true && true //true	
false && false //false
true && false //false
```

**OR Operator**

Similarly to the AND operator the OR, `||` operator returns true when either Boolean value is `true`.

```javascript
true || true //true	
false || false //false
true || false //true
```

```javascript
rue && false || true 
// true

false || false && true
// false

5 || 5
// 5

5 || 0
// 5

5 && 100
// 100

50 && 100 && 0 || 5
// 5 

10 || 0 || 5 && 15
// 10

```



**NOT operator**

The `!` operator returns `false` when the input is `true`. It returns `true` when the input is false.

```javascript
!true  //false
!false //true
```



## Undefined

In JavaScript, a variable without a value, has the value `undefined`. The type is also `undefined`.

```javascript
var car;    // Value is undefined, type is undefined
```

Any variable can be emptied, by setting the value to `undefined`. The type will also be `undefined`.

```javascript
car = undefined;    // Value is undefined, type is undefined
```

## Null

In JavaScript `null` is "nothing". It is supposed to be something that doesn't exist.

```javascript
var person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};
person = null;    // Now value is null, but type is still an object
```

## Difference Between Undefined and Null

```javascript
typeof undefined           // undefined
typeof null                // object

null === undefined         // false
null == undefined          // true
```


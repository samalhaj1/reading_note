# JavaScript Operators

**Example**

***Assign values to variables and add them together:***

var x = 5;          // assign the value 5 to x


var y = 2;         // assign the value 2 to y

var z = x + y;     // assign the value 7 to z (5 + 2)

The assignment operator (=) assigns a value to a variable.

**Assignment**

var x = 10;

The addition operator (+) adds numbers:

**Adding**

var x = 5;

var y = 2;

var z = x + y;

The multiplication operator (*) multiplies numbers.


**Multiplying**

var x = 5;

var y = 2;

var z = x * y;

## JavaScript Arithmetic Operators

**Arithmetic operators are used to perform arithmetic on numbers:**

|Operator|Description |
|--------|------------|
|+	|Addition
|-	|Subtraction
|*	|Multiplication
|**|	Exponentiation (ES2016)
|/|	Division
|%	|Modulus (Division Remainder)
|++	|Increment
|--|	Decrement


## JavaScript Assignment Operators

**Assignment operators assign values to JavaScript variables.**

|Operator|	Example|	Same As|
|--------|---------|---------|
|=	| x = y|	x = y
|+=	|  x += y|	x = x + y
|-=	|x -= y|	x = x - y
|*=	| x *= y|	x = x * y
|/=	|x /= y|	x = x / y
|%=	|x %= y|	x = x % y
|**= |	x **= y|	x = x ** y

The addition assignment operator (+=) adds a value to a variable.

Assignment

var x = 10;

x += 5;



## JavaScript String Operators

***The + operator can also be used to add (concatenate) strings.***

**Example**

var txt1 = "John";

var txt2 = "Doe";

var txt3 = txt1 + " " + txt2;

**The result of txt3 will be:**

**John Doe**

The += assignment operator can also be used to add (concatenate) strings:

Example
var txt1 = "What a very ";
txt1 += "nice day";
The result of txt1 will be:

What a very nice day

When used on strings, the + operator is called the concatenation operator.

## JavaScript Comparison Operators

|Operator|	Description|
|-------|-----------|
|==	|equal to
|===|	equal value and equal type
|!=	|not equal
|!==|	not equal value or not equal type
|>	|greater than
|<|	less than
|>=|	greater than or equal to
|<=|	less than or equal to
|?|	ternary operator

## JavaScript Logical Operators

|Operator|	Description|
|--------|-------------|
|&&	|logical and|
| \ \	|logical or|
|!	|logical not

# JavaScript Functions
A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

**Example**

function myFunction(p1, p2) {

  return p1 * p2;   // The function returns the product of

  p1 and p2
}

### JavaScript Function Syntax

A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().

Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

The parentheses may include parameter names separated by commas:

(parameter1, parameter2, ...)

The code to be executed, by the function, is placed inside curly brackets: {}

function name(parameter1, parameter2, parameter3) {
  // code to be executed

}

Function parameters are listed inside the parentheses () in the function definition.

Function arguments are the values received by the function when it is invoked.

Inside the function, the arguments (the parameters) behave as local variables.

A Function is much the same as a Procedure or a Subroutine, in other programming languages.

### Function Invocation

The code inside the function will execute when "something" invokes (calls) the function:

When an event occurs (when a user clicks a button)

When it is invoked (called) from JavaScript code
Automatically (self invoked)

You will learn a lot more about function invocation later in this tutorial.

### Function Return

When JavaScript reaches a return statement, the function will stop executing.

If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.

Functions often compute a return value. The return value is "returned" back to the "caller":

**Example**

Calculate the product of two numbers, and return the result:

var x = myFunction(4, 3);   // Function is called, return

 value will end up in x

function myFunction(a, b) {

  return a * b;             // Function returns the product
  
   of a and b

}

**The result in x will be:
12**

## Why Functions?

You can reuse code: Define the code once, and use it many times.

You can use the same code many times with different arguments, to produce different results.

**Example**

Convert Fahrenheit to Celsius:

function toCelsius(fahrenheit) {

  return (5/9) * (fahrenheit-32);

}

document.getElementById("demo").innerHTML = toCelsius(77);

***The ( ) Operator Invokes the Function***

Using the example above, toCelsius refers to the function

 object, and toCelsius() refers to the function result.

Accessing a function without () will return the function object instead of the function result.

**Example**

function toCelsius(fahrenheit) {

  return (5/9) * (fahrenheit-32);

}

document.getElementById("demo").innerHTML = toCelsius;
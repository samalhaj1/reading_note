

# JavaScript Arithmetic Operators


***Arithmetic operators are used to perform arithmetic between variables and/or values.***



class    |   Operator   |  Description |
-------  |   -------        --------
1.       |  +       	  |    Addition  |
2.       |  *           |  Multiplication |
3.       |   /          |  division    |
4.       |  %           | Modulus (division remainder)|
5.       | ++           | Increment|
6.       | _ _          | Decrement|


## JavaScript Assignment Operators
*Assignment operators are used to assign values to JavaScript variables.*

## JavaScript String Operators

*The + operator, and the += operator can also be used to concatenate (add) strings.*

#### Given that text1 = "Good ", text2 = "Morning", and text3 = "", the table below explains the operators:

 
 class    |Operator  | 	Example | 	text1 |	 text2 | 	text3|	
 -----    |  -----   |   -----  |   ----- | -----  |  -----|
  1.      |  +       |	text3 = text1 + text2 |"Good"|"morning" |"Good Morning"|
  2.    | + = | text1 += text2| "Good Morning"|"Morning"|	""|	



## Comparison Operators
*Comparison operators are used in logical statements to determine equality or difference between variables or values.*

#### Given that x = 5, the table below explains the comparison operators:


  |      |Operator|	Description|	Comparing|	Returns|
        | -----      |-------      |   --------  |  -------
 1.      |==      |	equal to   |	x == 8   |	false	|
 2.     |  |       |  x == 5   |true    |
 3.     | ===    | equal value and equal type| x === "5"| false |
 4.     |   |       | x === 5  |true|
 6.     | !=     | not equal  |x != 8      |true|
 7.     | !==    |not equal value or not equal type|x!=="5"|true|
 8.     |   |      |x!== 5| false|
 9.      | >      |greater than|x>8   |false|
 10.     |<       |less than   |x< 8  |true|
 11.    |>=      |greater than or equal to| x>=8|true|
 12.    |<=      |less than or equal| x<=8|true|


## Loops: while and for

#### We often need to **repeat actions**.

**For example**, outputting goods from a list one after another or just running the same code for each number from 1 to 10.

**Loops** are a way to ***repeat*** the same code multiple times.

**The “while” loop**

The while loop has the following syntax:

**while** (condition) {
  // code
  // so-called "loop body"
}

**While** the condition is truthy, the code from the loop body is executed.

A single execution of the loop body is called an iteration. The loop in the example above makes three iterations.

For instance, the loop below outputs i while i < 3:

let i = 0;
while (i < 3) { // shows 0, then 1, then 2
  alert( i );
  i++;
}

If **i++** was missing from the example above, the loop would repeat (in theory) forever. In practice, the browser provides ways to stop such loops, and in server-side JavaScript, we can kill the process.

Any expression or variable can be a loop condition, not just comparisons: the condition is evaluated and converted to a boolean by while.

## The “for” loop

The **for** loop is more complex, but it’s also the most commonly used loop.

#### It looks like this:

for (begin; condition; step) {
  // ... loop body ...
}


Let’s learn the meaning of these parts by **example**. The loop below runs alert(i) for i from 0 up to (but not including) 3:

**for** (let i = 0; i < 3; i++) { // shows 0, then 1, then 2
  alert(i);
}

|part|        |
|-----|	
|begin|	i = 0  |	Executes once upon entering the loop.
|condition|	i < 3|	Checked before every loop iteration. If false, the loop stops.
|body|	alert(i)|	Runs again and again while the condition is truthy.
|step	|i++|	Executes after the body on each iteration.

**The general loop algorithm works like this:**  


  Run begin
→ (if condition → run body and run step)
→ (if condition → run body and run step)
→ (if condition → run body and run step)
→ ...

That is, begin executes once, and then it iterates: after each condition test, body and step are executed.

If you are new to loops, it could help to go back to the example and reproduce how it runs step-by-step on a piece of paper.

**Here’s exactly what happens in our case:**

// for (let i = 0; i < 3; i++) alert(i)

// run begin

let i = 0

// if condition → run body and run step

if (i < 3) { alert(i); i++ }

// if condition → run body and run step

if (i < 3) { alert(i); i++ }

// if condition → run body and run step

if (i < 3) { alert(i); i++ }

// ...finish, because now i == 3



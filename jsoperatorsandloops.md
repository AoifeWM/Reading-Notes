# Operators and Loops in Javascript

Operators and Loops are important tools in any programming language. Many of them are structured similarly across multiple languages, but today we'll be discussing how they're structured in javascript.

## Operators

Operators are used to assign new values to variables, or compare them to each other. They're important in many different applications. Here are some of the most important assignment operators in javascript:

* `x = y`: sets x to y
* `x += y`: shorthand to set x equal to (x+y)
* `x -= y`: shorthand to set x equal to (x-y)
* `x *= y`: shorthand to set x equal to (x*y)
* `x /= y`: shorthand to set x equal to (x/y)
* `x %= y`: shorthand to set x equal to the *remainder* of (x/y)
* `x **= y`: shorthand to set x equal to x to the power of y
* `x &= y`: shorthand to set x equal to the boolean value of (x AND y)
* `x ^= y`: shorthand to set x equal to the boolean value of (x XOR y)
* `x |= y`: shorthand to set x equal to the boolean value of (x OR y)
* `x++`: shorthand to set x equal to (x+1)
* `x--`: shorthand to set x equal to (x-1)

Here are some of the most important comparison operators in javascript:

* `x == y`: will return `true` if x equals y (*does not* have to be the same type of variable, for instance, when `x = 1` (1 as an integer) and `y = '1'` (1 as a string) this operation will return `true`)
* `x === y`: will return `true` if x equals y (*does* have to be the same type of variable, for instance, when `x = 1` and `y = '1'` this operation will return `false`)
* `x != y`: will return `true` if x does *not* equal y (*does not* have to be the same type of variable, for instance, when `x = 1` and `y = '1'` this operation will return `false`)
* `x != y`: will return `true` if x does *not* equal y (*does* have to be the same type of variable, for instance, when `x = 1` and `y = '1'` this operation will return `true` because they aren't the same type of variable)
* `x >= y`: will return `true` if x is greater than or equal to y
* `x <= y`: will return `true` if x is less than or equal to y
* `x > y`: will return `true` if x is greater than y
* `x < y`: will return `true` if x is less than y

There are also basic arithmetic operators which can be used in equations, including *, +, -, and /. Here are some other arithmetic operators:

* `**`: calculates something to the power of another thing, often written on paper as ^
* `%`: calculates the remainder of one divided by another, for instance, `17 % 5` will be calculated as 2.

## Loops and Iteration

Loops are an important tool used in coding. They can repeat certain actions based on defined conditions; for instance, you may set them up to repeat a certain number of times, to repeat until a certain condition is reached, or to repeat indefinitely. The two most important fundemental types of loops are `for` and `while`.

### While Loops

A while loop will repeat indefinitely until a certain condition is reached. It is structured like this:
`while([condition]){[code to be executed]}`
The condition will be a boolean statement that will return either `true` or `false`; as long as it returns true, the loop will continue repeating. Each time the [code to be executed] is completed, the while loop checks again if the condition is met, and decides whether to loop again or not. If the condition is not met the first time the while loop is reached by the computer, the while loop will never execute.
For example, if you set the [condition] to `1==1`, the loop will repeat forever, as `1==1` will always return true, and conversely if you set it to `1==0` the while loop will never execute.
While loops are useful for situations where you want the code to repeat no matter what until a condition is fulfilled, for instance, until the right password is input.

#### Do While Loops

A `do ... while` loop is very similar to a while loop, but it will execute at least once no matter what. It runs the [code to be executed] one time, and *then* checks the [condition] to see if it should run again. It is structured like this:
`do{[code to be executed]}while([condition])`

### For loops

For loops are like while loops but they have inbuilt condition to track how many times they've run. When a for loop is initiated, it runs a statement to set up a variable. After that, and each time the loop repeats, it checks a condition just like a while loop, and decides if it should run based on whether that condition returns true or false. After completing each iteration, it runs an *incrementing* statement to change the variable set up initially. It is structured like this:
`for([initial statement], [condition], [incrementing statement]){[code to be executed]}`
Here's an example for loop:
`for(let i = 0; i < 10; i++;){alert(i.value)}`
This loop will make the variable `i`, and set it to 0. Then, it checks if `i` is less than ten; it is, so it executes `alert(i.value)` and sends an alert displaying the value of i. Then it increments `i` by one because of the `i++` statement, making `i` equal 1. It checks the condition again; `i` is still less than 10, so it sends the alert, increments `i` by one again, and then checks the condition which returns true again, and so on and so forth, until `i` reaches 10 and the loop stops. This code will send a series of 10 alerts showing the numbers 0-9.
For loops are useful for when you want a piece of code to repeat a descrete number of times, and no more. The condition can also be based on other variables; for instance, if you want the user to decide how many times the loop runs, you can prompt them for a variable and then set the condition to `i < userVariable;`.

## Break

Break is a statement that will end the current loop, regardless of whether its conditions have been met. For instance, even a `while(1==1)` can be ended with the statement `break;`. Break will only break the current loop it is in, so if that loop is inside another loop, the outside loop will continue going.

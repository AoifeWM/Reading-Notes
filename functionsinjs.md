# Functions in javascript

Javascript has a tool availiable in many programming languages called functions. Functions are individual packets of code that can be activated ('invoked' or 'called') many other times. Functions make code cleaner and more legible, recursion easier, and can save processing power and disk space when one chunk of code must be used in many places.

## Inputs and Outputs in functions

Functions can be set up to accept inputs and return outputs to other functions. These inputs are defined in round brackets at the start of the function, for instance, in `function example`**`(var1)`**`{[some code goes here]}` the variable var1 is an input which can be used in the code of the function (which is contained in the squigly brackets). To output code, the function can make a **return** statement, for example, `function double(var1){let result = var1 * 2; return result;}` the variable result will be returned. Functions are called by typing the name of the function, plus round brackets, and within the round brackets should be any apropriate variables. This can be used in another piece of code; for example, if you want to make a new variable equal to 5*2 and add 3, you could run `let newVar = 3 + double(5);`. When the code encounters the reference to the function `double`, it will run `double` using 5 as the value of var1, and then compute the rest of the equation by substituting the call to `double` with the **returned** value (in this case 10), setting `newVar` to 13. This is a simple example, but functions can be much more complicated, and can call other functions within themselves (or even call themselves). Functions can also take more than one input value, seperated by commas in the round brackets at the start.
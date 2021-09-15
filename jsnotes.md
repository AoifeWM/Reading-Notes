# Javascript

Javascript is a language designed to add functionality to a webpage which is not covered in html, and can be used for many complicated purposes. It can be used for other purposes as well, but for now we will be covering its use in webpages. It can handle variables, logic loops, mathematics, and much more.

## Input and output in javascript

Javascript can interact directly with the working HTML document. Using elements like `input` in HTML, javascript can take user input and do various things with it. An easy way to do this is assign a unique ID to the input element and then use the `document.getElementById([ID of the chosen field])` function in javascript to assign it to a javascript variable. Javascript can also write directly to the HTML document with the `document.write` function or by altering the `document.getElementByID()` as if it's a variable.

## Variables in JS

Variables can be constructed in 3 ways in javascript, with `var [variable] = ...`, `let [variable] = ...` and `const [variable] = ...`, however the last two are often the best practice and `var` can be ignored. `let` and `const` should be used differently; `let` is for variables which may change and `const` is for variables which will remain static. These variables can be altered (`[variable] = [new value]`, `[variable] += [another value to be added]`, `[variable] -= [another value to be subtracted]`), compared (with functions like `==`, `>=`, or `<=`), or used in equations (ie. `variable1 + variable2`, `var1 * var2`, etc.). Variables may be strings (text), integers, floats (numbers with decimals), dates, boolean (true/false) values, and more. They can even be undefined, having no variable type assigned to them yet. Variable names can use uppercase and lowercase letters, underscores (_), and dollar signs ($).

## Logic in JS

Logic loops can be constructed in javascript using the elements `if([condition]{}` and the code inside the squigly brackets will only be exectured if the condition is met (returns `true`); They can also be appended with `else{}` or `elseif(condition 2){}` which are only executed if the first condition isn't met, or if the first condition isn't met and the second condition is, respectively.

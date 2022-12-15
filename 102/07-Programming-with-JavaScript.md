# 07 - Programming with JavaScript

## Control Flow

the order in which the computer executes  

## Control structure

- conditioal
    > if (???) {???;} else {???;}

- loops
    > iterates through all of the fields in the form, checking each one in turn
- functions

## JavaScript Functions [^1]

- is a block of code designed to perform a particular task  
- is executed when "something" invokes it (calls it)  

> function **function-name**(parameter1,parameter2...) {code to be executed}  

### ` **name** is the **function object**, and **name()** refers to the **function result**.`

* Accessing a function without () will return the function object instead of the function result.
*Function **arguments** are the **values** received by the function when it is invoked.

*Inside the function, the arguments (the parameters) behave as local variables.

### Function Invocation

The code inside the function will execute when "something" invokes (calls) the function:

- When an event occurs (when a user clicks a button)  
- When it is invoked (called) from JavaScript code  
- Automatically (self invoked)  

### Function Return *always at the end iof function)

- When JavaScript reaches a `return` statement, the function will stop executing.

- If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.

- Functions often compute a **return value**. The return value is "returned" back to the "caller"

#### Functions can be Used as Variable Values
 > let text = "The temperature is " + toCelsius(77) + " Celsius";

### Local Variables

Variables declared within a JavaScript function, become LOCAL to the function.

Local variables can only be accessed from within the function.

> *// code here can NOT use carName*  
function myFunction() {
  let carName = "Volvo";  
  *// code here CAN use carName*
}  
*// code here can NOT use carName*

*variables with the same name can be used in different functions.  
*Local variables are created when a function starts, and deleted when the function is completed.

## JavaScript Operators[^2]

- Assignment Operator (=) assigns a value to a variable

- Addition Operator (+) adds numbers

- Multiplication Operator (*) multiplies number

### Types of JavaScript Operators

- Arithmetic Operators (math problems) 
  - `+`
  - `-`
  - `*`
  - `**`Exponentiation
  - `/`
  - `%`Modulus (Division Remainder)
  - `++`Increment
  - `--`Decrement
- Assignment Operators (assign values to JavaScript variables)
  - Addition Assignment Operator (+=) adds a value to a variable
- Comparison Operators
  - `==` equal to
  - `===` equal value and equal type
    - `!=` not equal
    - `!==` not equal value or not equal type
    - `>` greater than
    - `<` less than
    - `>=` greater than or equal to
    - `<=` less than or equal to
    - `?` ternary operator
- Logical Operators
  - `&&` logical and
  - `||` logical or
  - `!` logical not
- Conditional Operators
- Type Operators
  - `typeof` Returns the type of a variable
  - `instanceof` Returns true if an object is an instance of an object type
- JavaScript Bitwise Operators

### The precedence of operators determines the order they are applied when evaluating an expression.  

>For example:  
const x = 1 + 2 * 3;  
const y = 2 * 3 + 1;

Despite * and + coming in different orders, both expressions would result in 7 because * has precedence over +, so the *-joined expression will always be evaluated first.


## additional resources:

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators

[^1]: https://www.w3schools.com/js/js_functions.asp

[^2]: https://www.w3schools.com/js/js_operators.asp
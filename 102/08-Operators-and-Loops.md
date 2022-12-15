# 08 - Operators and Loops

* you can write html inside a string  

> `document.write("<img src='link' alt='alt text'/>")`

* Logical AND `&&`
* Logical OR `||`
* Logical NOT `!`

eg:
> let a = 5;  
let b = '5';  
console.log((a == b) && (b > a))

True && False > False 

# Expressions and operators [^1]

 an expression is a valid unit of code that resolves to a value.  
 there are 2 types of expression:
 - those that have side effects (such as assigning values)
   - x = 7  
 - those that purely evaluate.
   - 3 + 4
   > This expression uses the + operator to add 3 and 4 together and produces a value, 7. However, if it's not eventually part of a bigger construct (for example, a variable declaration like const z = 3 + 4), its result will be immediately discarded — this is usually a programmer mistake because the evaluation doesn't produce any effects.

## Assignment operators

- x = f() > x = f()
- x += f() > x = x + f()
- x -= f() > x = x - f()
- `* or / or % or **`
- x <<= f() > x = x << f()  (left shift)
- x &= f() > x = x & f() (Bitwise AND)
- 	x ^= f() > x = x ^ f() (Bitwise XOR)
...

## Comparison operator

compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values.

 In most cases, if the two operands are not of the same type, JavaScript attempts to convert them to an appropriate type for the comparison. 

 *The sole exceptions to type conversion within comparisons involve the === and !== operators, which perform strict equality and inequality comparisons.

   - `==` equal to
  - `===` equal value and equal type (Strict equal)
  - `!=` not equal
  - `!==` not equal value or not equal type
  - `>` greater than
  - `<` less than
  - `>=` greater than or equal to
  - `<=` less than or equal to
  - `?` ternary operator

# Loops [^2]

they repeat an action some number of times

## for statement

A for loop repeats until a specified condition evaluates to false. 

> `for ([initialExpression]; [conditionExpression]; [incrementExpression])`  
  `statement`

> `for (initial value; condition to evaluate; increment)`  
`{code to execute}`

1. **initialExpression**: This expression usually initializes one or more loop counters

2. **conditionExpression**: if "true", the loop statements execute. if "not true", `for` loop terminates.  
(If the conditionExpression expression is omitted entirely, the condition is assumed to be true.)

3. **statement**: executes

4. If present, the update expression `incrementExpression` is executed.

5. Control returns to 2.

## while statement

A while statement executes its statements as long as a specified condition evaluates to true.  
*It will keep going until the condition is false.

> `while (condition)`  
  `statement`

> `while (the evaluates to true) {execute this code}`

If the `condition` becomes "false", `statement` within the loop stops executing and control passes to the statement following the loop.

The condition test occurs before `statement` in the loop is executed. If the condition returns "true", `statement` is executed and the `condition` is tested again. If the condition returns "false", execution stops, and control is passed to the statement following `while`.

To execute multiple statements, use a block statement (`{ }`) to group those statements.

let x = 5;  
while (x < 3){  
    console.log(x);  
    x += 1;  
}

[^1]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators

[^2]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration
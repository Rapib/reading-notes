# 06 - Dynamic web pages with JavaScript

## JavaScript is a  
- ightweight  
- interpreted  
- or just-in-time  
compiled programming language.

*not just websites use it, eg Node.js, Apache CoucgDB, Adove Acrobat.

It is  
- prototype-based  
- multi-paradigm  
- single-threaded  
- dynamic language  
- supporting object-oriented  
- imperative  
- declarative (e.g. functional programming) styles.  

JS =/= Java

## 3 major parts of JS

1. the language  
2. DOM API (how the language can interact with parts of a web page)
3. (server) API, provided by Node.js...

## Embed or include JS

- embed (inside html file)
- included (put a link in html and link it to a js file ~CSS)

>  `<script> code </script>`

## output or input JS
eg of output  
> `<script language="javascript">`
 `alert("Hello World");`  
 `</script>`
 
 eg of input  [^1]  
> `<script>`  
`var name = prompt("Your name:", "");`  
`document.write("Hello ", name);`  
`</script>`




## 4 Ways to Declare a JavaScript Variable (= containers for storing data,numbers / text strings):

- Using var  
- Using let  <let can be changed>
- Using const <cant be changed> 
- Using nothing  

>If you want a general rule: always declare variables with const.

> If you think the value of the variable can change, use let.[^2]

**Variables must be identified with unique names, which are called identifiers* & case-sensitive

## equal sign (=) is an "assignment" operator, not an "equal to" operator.

* "equal to" operator is written like `==` in JavaScript.

## examples

> let greeting = "hello"  
then  
let greeting ="abc"  
NO GO because greeting = hello already,  
but if we change it to greeting = "abc" without let, it will work


* treat number as text use `"1"`

> "1" + "3"  => 13  
> 1 + 3 => 4  
> "1" + 3 => 13

[^1]: https://code-maven.com/javascript-input-with-prompt-and-confirm]

[^2]: https://www.w3schools.com/js/js_variables.asp
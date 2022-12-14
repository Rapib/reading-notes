# 05 - Design web pages with CSS

## CSS (Cascading Style Sheets)

html is a mark up doc with very basic styles.  
CSS is a language for specifying how **documents** (a text file structure using a markup language, eg html, XML, SVG) are **presented** (coverting a doc into a form usable by your audience. Browsers aka user agent are designed to do that) to a user

*CSS can be used to change the text styling, create a layout, effects


## CSS can be written in 3 ways [^1]

- ### external (.css file without html tags)
(separate CSS file connected to html.  
 *Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section.*)

 > `<html>`  
`<head>`  
***`<link rel="stylesheet" href="mystyle.css">`***  
`</head>`  
`<body>....`

*External styles are defined within the <link> element, inside the <head> section of an HTML page

> `body {`  
  `background-color: lightblue;`  
`}`

sample of a css file


- ### internal (built into the html file)

(is defined inside the `<style>` element, inside the head section)

>  `<html>`  
`<head>`  
`<style>`  
`body {`  
`  background-color: linen;`  
`}`  
`h1 {`  
  `color: maroon;`  
  `margin-left: 40px;`  
`}`  
`</style>`  
`</head>`  
`<body>`  
`<h1>This is a heading</h1>`  
`<p>This is a paragraph.</p>`  
`</body>`  
`</html>`  


- ### inline (inside html element)

> `<h1 style="color:blue;text-align:center;">This is a heading</h1>`  
or  
`<p style="color:red;">This is a paragraph.</p>`  

## CSS syntax

CSS is a rule-based language. telling which group to have what style

eg. 

>selector {      
    property: value;  
    property: value;  
    property: value;  
    }

eg2.

>h1 {  
  color: red;  
  font-size: 5em  ;
}

Telling heading h1 to have large red text.  
selector = h1  
then have `curly braces { }`  
declarations, in the form of property & value PAIR  

## Cascading Order
if there is more than 1 style for an html element, number 1 will has the highest priority:

1. Inline style (inside an HTML element)  
2. Internal style sheets (in the head section)  
3. External style sheets
4. Browser default


## Classes `.` are for multiple elements 
> `<section class="lower">` <- html>
`.lower  {width: 30%;}` <- css> 
## IDs `#` needs to be unique
> #id {....} <- css  
`<img id="id"....>` <- html
> `section {display: inline-block;}` <- css    

parallel block

## Other CSS

> `nav ul {text-decoration: none; list-style: none;}`  

remove the dot in front of the links

> `nav li {display: inline-block;}`

parallel nav link

> `body {margin: 20px;}`

create margin

>`#img {float: left;}`

txt wrap around pic

[^1]: https://www.w3schools.com/css/css_howto.asp

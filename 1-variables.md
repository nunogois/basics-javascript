# Variables

JavaScript is a dynamic **untyped** language which means you just declare variables without specifying their type (text, number, etc).

This can be a *double-edged sword*. It is easy to learn and code in, but it can also sometimes lead to nasty bugs and unexpected behaviour if you're not careful.

### Declaring variables - var

```JavaScript
console.log("Hi! The console.log function helps us print output. Feel free to run these examples in your browser's console.")
console.log("You may also type a variable name in your browser after declaring it to return its value.")

var variable = '<- This is a variable that is holding this text as value'
console.log(variable) // the variable's content will be printed in the console

// Text variables are very common and text can be represented with either ' or "
var text1 = 'This is a text'
var text2 = "This is also a text"

// Like in other programming languages, you can escape characters (explicit literals) with \
var text3 = 'This is a text with "\'" but that\'s ok because we\'re properly escaping the content!'
var text4 = "It is also perfectly fine to have \" in here!"
console.log(text3, text4)

// Number variables are also very common
var lucky_number = 7
var ten = lucky_number + 3
console.log(lucky_number, ten)

// And so is concatenating - joining content!
var name = 'Nuno'
var age = 31
var year = 2021
var sentence = 'Hi! My name is ' + name + ' and in the year ' + year + ' I am ' + age + ' years old. Starting to feel old!'

console.log(sentence)

// A variable that has been declared but has no value, is undefined
var no_value
console.log(no_value)

// A variable that is used but hasn't been declared, gives out an error
console.log(something_else)
```

### Declaring variables - let, const

```JavaScript
/* 
Declaring variables with let and const may not be available in your environment. 
If you're using them directly in your front-end without something like Babel you may face some issues on older browsers. 
*/

let info = 'let is the preferred way of declaring variables, assuming your environment allows it.'
const constant = 'this is a constant that may not be changed. Try declaring a const and then changing its value. Nope!'
```

### Common variable types

```JavaScript
let questionmark = undefined // Undefined: the same as not setting a value
let nothing = null // Null: nothing
let text = 'Hello World' // Text: string of characters
let number = 1 // Number: can also have decimal places - 13.37
let bool = true // Boolean: true / false
let array = [] // Array: a list of values
let json = {} // JSON: a complex object
```

We will explore these variable types in the next chapters.

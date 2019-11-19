[![General Assembly Logo](https://camo.githubusercontent.com/1a91b05b8f4d44b5bbfb83abac2b0996d8e26c92/687474703a2f2f692e696d6775722e636f6d2f6b6538555354712e706e67)](https://generalassemb.ly)

# Warmup

#### Learning Objectives

- Practice using conditionals.

#### Prerequisites

- Introductory lesson to JavaScript

---



## Directions
Write  `if`, or `if, else` statements to complete the following questions. Some of the problems may require you to use a  conditional. Refer back to your class notes from today if you need help.

## Conceptual Questions

Rate your understanding of the following questions on a scale of 1 - 5. If your understanding is less than or equal to 3, research the answer or ask for help:

1. How do we assign a value to a variable?
  - Which line(s) is/are valid? all except the third

    ```js
    let a = 0;   \\works
    const b = 1; \\works
    9 = a;       \\doesn't work
    b = b + 5;   \\works
    ```

2. How do we change the value of a variable? reassign it if not a const
3. How do we assign an existing variable to a new variable? initialize the value and assign the old to the new

## Let's get Mathy!

```js
const a = 42.78
const b = 1.1
const c = -2
const d = .5
const e = 16
```

- Round `a` down floor(a) = 42
- Round `b` up ceil(b) = 2
- Find the absolute value of `b - a` abs(b-a) = 41
- Find the square root of `e` sqrt(16) = 4
- Raise `e` to the power of `d` e^d = sqrt(16) = 4
- Make a digital die 0 generate a random number between 1 - 6 Math.floor(Math.random() *6) + 1 

## Strings Activity 1

### Strings - Switcharoo
1. Create a variable called `firstVariable`. var firstVariable = "Hello World"; firstVariable = 1; var secondVariable = firstVariable; secondVariable = string(secondVariable); // value of firstVariable is 1
1. assign it the value of a string: `"Hello World"`
1. On the next line, change the value of this variable to a number.
1. store the value of `firstVariable` into a new variable called `secondVariable`
1. On the next line, change the value of `secondVariable` to a string.
1. What is the value of `firstVariable`?

```js
var firstVariable = "Hello World"; 
firstVariable = 1; 
var secondVariable = firstVariable; 
secondVariable = string(secondVariable); 
// value of firstVariable is 1
```

### Strings - Combine it
1. Create a variable called `yourName` and set it equal to your name as a string.
  - Write an expression that takes the string "Hello, my name is " and the variable `yourName` so that it prints a new string with them concatenated

```js
var yourName = "Mohammed"
var str = "Hello, my name is " + yourName 
```

>ex: `Hello, my name is Jean Valjean`

## Booleans Activity
- Using the provided variable definitions, replace the blanks with a mathematical or boolean operator **that evaluates the expression to true**.

[MDN Comparison Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators)

```
  const a = 6;
  const b = 100;
  const c = -5;
  const d = 3000;
  const e = 'Jelly Bean';
```

1.  a < b;
1.  c < d;
1.  'Peanut' === 'Peanut';
1.  a < b > c;
1.  a === a < d;
1.  e === 'Jelly Bean';
1.  48 != '48';
1. 'e' < 'Eh' || 'e' !== 'Eh'

## The Age Calculator

Forgot how old someone is? Calculate it!

- Store the current year in a variable.
- Store their birth year in a variable.
- Calculate their 2 possible ages based on the stored values.
- Output them to the screen like so: "They are either NN or NN", substituting the values.

// The Age Calculator
// Forgot how old someone is? Calculate it!

// Store the current year in a variable.
// Store their birth year in a variable.
// Calculate their 2 possible ages based on the stored values.
// Output them to the screen like so: "They are either NN or NN", substituting the values.

```js
var currYear = 2019
var dob = 2000
var age = currYear - dob
console.log("Thet are either " + age - 1 + " or " + age
```

## The World Translator
// Write an if statement that writes Hello World in different languages (i.e. if the language is English, print `"Hello World"`, if the language is Arabic write something `"مرحبا بالعالم"`, if the language is French write something romantic)

```js
var language = 'Arabic'
if(language === 'English) console.log("Hello World!")
else if (language === 'Arabic') console.log("العالم يرحب فيك")
else if (language === 'French') console.log("De Rien")
```
 ## Driving Age
// - Store the user age
// - If age is less than 18, print "Sorry, you can't drive yet"
// - If the age is equal to or over 18, print "Drive away!"
// - Bonus: If the user can't drive yet, tell them how many years they will have to wait. E.g. "Sorry, you have 4 years to wait until you can drive"

```js
var input = prompt("enter your age: ")
if (input < 18) {
  console.log("Sorry, you can't drive yet")
  var date = new Date()
  var currYear = date.getFullYear()
  var leftYears = currYear - input
  console.log("Sorry, you have around " + leftYears + " years to wait until you can drive")
}
else if (input >= 18) console.log("Drive away!")
```

## The Temperature Converter
// It's hot out! Let's make a converter based on the steps here.
// Store a celsius temperature into a variable.
// Convert it to fahrenheit and output "NN°C is NN°F".
// Now store a fahrenheit temperature into a variable.
// Convert it to celsius and output "NN°F is NN°C."

```js
var tempC = 30
var tempCToF = ( tempC *  9/5) + 32
console.log(tempC + "°C is " + tempCToF + "°F"
var tempFToC = (tempCToF − 32) * 5/9
console.log(tempCToF + "°F is " + tempFToC  + "°C."
```

## The Fortune Teller
// Why pay a fortune teller when you can just program your fortune yourself?

// Store the following into variables: number of children, partner's name, geographic location, job title. Output your fortune to the screen like so: "You will be a X in Y, and married to Z with N kids."

```js
const person = {
  numOfChildren : 5,
  parentName : "Someone",
  location : "Jeddah",
  jobTitle : "SEI student"
}
console.log("You will be a " + person.jobTitle + " in " + person.location + ", and married to " + person.parentName + " with " + person.numOfChildren + " kids."
```

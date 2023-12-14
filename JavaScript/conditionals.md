
# Conditionals
## Falsy values: 
* false
* 0
* ''
* null
* undefined
* NaN

## Truthy values:
* [] - empty array

# == Vs ===
* == - converts the variable values to the same type before performing
  comparison. This is called type coercion.
* === - does not do any type conversion (coercion) and returns true only if
  both values and types are identical for the two variables being compared.



* Comparing two JavaScript objects always returns false.
`== -> false `  and `=== -> false` 



# If, else if, else

```javascript
let x = 9;

if (x === 10) {
    console.log("x er 10")
} else if (x < 10) {
    console.log("x er mindre enn 10")
} else if (x > 10) {
    console.log("x er større enn 10")
} else {
    console.log("x er ikke en integer")

```

# Ternary operator
* `bool ? foo : bar`  - is interpreted as one unit. Hence, no nedd to use
  parenthesis to nest ternary operators:
  `bool ? ( bool ? foo : bar ) : baz`   *is the same as*   `bool ? bool ? foo : bar : baz` 
  But use parenthesis for readability.


## Same with ternary operator
* The ternary operator is right-associative, which means it can be "chained" in
  the following way, similar to an if … else if … else if … else chain:

```javascript

let x = 9;
x === 10 ? console.log("x er 10") : x < 10 ? console.log("x er mindre enn 10") : x > 10 ? console.log("x er større enn 10") : console.log("x er ikke en integer")

```

or

```javascript

x === 10
  ? console.log("x er 10")
  : x < 10
  ? console.log("x er mindre enn 10")
  : x > 10
  ? console.log("x er større enn 10")
  : console.log("x er ikke en integer");
```



# Ternary operator - Cool examples
## Printing with ternary operator
```javascript
console.log(age >= 18 ? "Ta deg en øl din voksne person" : "Ta deg en juice din unge")
```

## Assign value to variable
```javascript
const beverage = age >= 21 ? "Beer" : "Juice";
```


## Handeling null values
```javascript
const greeting = (person) => {
  const name = person ? person.name : "stranger";
  return `Howdy, ${name}`;
};

console.log(greeting({ name: "Alice" })); // "Howdy, Alice"
console.log(greeting(null)); // "Howdy, stranger"
```



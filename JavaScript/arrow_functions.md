
# Arrow function
* **The function is nameless but is assigned to a variable, hence use let or const keyword.**
* **No need for return** (implicit return) - If the function has only **one statement**, and the statement returns a value, you can remove the brackets and the return keyword.
* **No need for curly braces** - If the function has only one statement, you can remove the brackets.

# Arrow function vs normal function
```javascript
hello = function() {
  return "Hello World!";
}
```

```javascript
hello = () => {
  return "Hello World!";
}
```

* It gets shorter! If the function has only one statement, and the statement returns a value, you can remove the brackets and the return keyword:

```javascript
hello = () => "Hello World!";
```

* In fact, if you have only one parameter, you can skip the parentheses as well:

```javascript
hello = val => "Hello " + val;
```

# Problem: Return object from arrow function
* problem: object literal is interpreted as a block of code.
```javascript
let getBook = (id) => {id: id, name: 'Harry Potter'};
```

* solution: wrap the object literal in parentheses.
```javascript
let getBook = (id) => ({id: id, name: 'Harry Potter'});
```


# Anonymous Function - Normal function vs Arrow function

**Normal function**
```javascript
let anonymousFunction = function() {
    console.log('This is an anonymous function');
};
```
* The function is nameless but is assigned to a variable. 
* The variable can be used to call the function.


**Arrow function**
```javascript
let anonymousFunction = () => console.log('This is an anonymous function');
```




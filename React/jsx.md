
# jsx syntax


```javascript
const element = <h1>Hello, world!</h1>;
```
This funny tag syntax is neither a string nor HTML.
It is called JSX, and it is a syntax extension to JavaScript. 

* 'JSX produces React “elements”. 


* Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both.



# JavaScript in curly braces
```javascript
const name = 'Josh Perez';
const element = <h1>Hello, {name}</h1>;
```


# Multi-line JSX expressions
```javascript
const element = (
  <h1>
    Hello, {formatName(user)}!
  </h1>
);
```


* We split JSX over multiple lines for readability. While it isn’t required,
  when doing this, we also recommend wrapping it in parentheses to avoid the
  pitfalls of automatic semicolon insertion.


# Compilation - JSX is compiled to  
* After compilation, JSX expressions become regular JavaScript function calls
  and evaluate to JavaScript objects.
* This means that you can use JSX inside of if statements and for loops, assign
  it to variables, accept it as arguments, and return it from functions:




# JSX Prevents Injection Attacks

It is safe to embed user input in JSX:

```javascript
const title = response.potentiallyMaliciousInput;
// This is safe:
const element = <h1>{title}</h1>;
```

# React elements

* Babel compiles JSX down to React.createElement() calls.

These two examples are identical:

```javascript

const element = (
  <h1 className="greeting">
    Hello, world!
  </h1>
);
```
```javascript
pconst element = React.createElement(
  'h1',
  {className: 'greeting'},
  'Hello, world!'
);
```



**React.createElemnt**

React elemnt structure: 

```javascript
// Note: this structure is simplified
const element = {
  type: 'h1',
  props: {
    className: 'greeting',
    children: 'Hello, world!'
  }
};
```

React reads these objects and uses them to construct the DOM and keep it up to date.

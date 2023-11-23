



# Callback 
* A callback is a function passed as an argument to another function
* `setTimeout` - is a built-in function that calls a function after a certain period of time


## Example 1
* `myFunction`  is the callback function
```javascript
setTimeout(myFunction, 3000);
```
or 
```javascript
setTimeout(() => console.log("hello"), 3000);
```

## Example 2
**Bad:**
```javascript
function myDisplayer(some) {
  document.getElementById("demo").innerHTML = some;
}

function myCalculator(num1, num2) {
  let sum = num1 + num2;
  myDisplayer(sum);
}

myCalculator(5, 5);
```


**Good:** - functional programming style: 
```javascript
function myDisplayer(some) {
  document.getElementById("demo").innerHTML = some;
}

function myCalculator(num1, num2, myCallback) {
  let sum = num1 + num2;
  myCallback(sum);
}

myCalculator(5, 5, myDisplayer);
```




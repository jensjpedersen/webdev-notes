


# Typical d3 function call pattern

* call method is used to call a function on a selection

Parameters:
* callback function
* callback function arguments


```javascript


function functionName(arg1, arg2, ...) {
  // do something
}


const selection = d3.select('svg');
selection.call(functionName, arg1, arg2, ...)
```







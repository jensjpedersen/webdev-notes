


# Reduce
syntax: 
```javascript
reduce(callbackFn)
reduce(callbackFn, initialValue)
array.reduce(function(total, currentValue, currentIndex, arr), initialValue)
```

```javascript
let arr = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
const initialValue = 0; 
const result = arr.reduce((acc, curr, index, array) => acc + curr, initialValue)
console.log(result);
```


**Parameters:**
* initialValue Optional - A value to which accumulator is initialized the first time the callback is called. If initialValue is specified, callbackFn starts executing with the first value in the array as currentValue. If initialValue is not specified, accumulator is initialized to the first value in the array, and callbackFn starts executing with the second value in the array as currentValue. In this case, if the array is empty (so that there's no first value to return as accumulator), an error is thrown.

* callbackFn - A function to execute for each element in the array. Its return value becomes the value of the accumulator parameter on the next invocation of callbackFn. For the last invocation, the return value becomes the return value of reduce(). The function is called with the following arguments:
    * accumulator - The value resulting from the previous call to callbackFn. On the first call, its value is initialValue if the latter is specified; otherwise its value is array[0].
    * currentValue - The value of the current element. On the first call, its value is array[0] if initialValue is specified; otherwise its value is array[1].
    * currentIndex - The index position of currentValue in the array. On the first call, its value is 0 if initialValue is specified, otherwise 1.
    * array - The array reduce() was called upon.





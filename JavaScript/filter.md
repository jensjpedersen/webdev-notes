
# filter
* The filter() method is an iterative method. It calls a provided callbackFn
  function once for each element in an array, 
* **and constructs a new array of all the values for which callbackFn returns a truthy value.**

Syntax
```javascript
array.filter(function(currentValue, index, arr), thisValue)
```


## Example 1
```javascript
const ages = [32, 33, 16, 40];
const result = ages.filter(checkAdult);

function checkAdult(age) {
  return age >= 18;
}
```

## Example 2 - Illustration purpose 
* returns array elements associated with truty return value in callback. 
```javascript
let arr = [1,2,3,4,5,6,7,8,9,10]

function callbackFn(value) {
    if (value>5) {
        return true
    }
    else if (value == 1 ) {
        return true
    }
    else {
        return false
    }
}

console.log(arr.filter(callbackFn)); // [ 1, 6, 7, 8, 9, 10 ]
```


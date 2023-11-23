
# forEach
Syntax: 
```javascript
forEach(callbackFn)
forEach(callbackFn, thisArg)
```

* Parameters: `callbackFn` - Function to execute for each element, taking three arguments:
      * `currentValue` - The current element being processed in the array.
      * `index` - The index of the current element being processed in the array.
      * `array` - The array that forEach() is being applied to.
  * `thisArg` - Optional. Value to use as `this` when executing `callbackFn`.
* Does not return anything - Return: `undefined` 
* `forEach` takes a callback function as an argument
  and calls the callback function once for each element in the array

```javascript
const names = ['Alice', 'Bob', 'Charlie', 'Deborah', 'Evan'];

names.forEach((name) => console.log(name));
```


## Get element + index
```javascript
myArray.forEach(function (value, i) {
    console.log('%d: %s', i, value);
});
```


## Default parameters in callback
* item
* index
* arr

```javascript
const numbers = [65, 44, 12, 4];
numbers.forEach(myFunction)

function myFunction(item, index, arr) {
  arr[index] = item * 10;
}
```


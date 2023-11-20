
# Spread operator
* `...` is the spread operator
* Used to quickly copy all or part of an existing array or object into another array or object.
* It expands a string into an array of characters
* Works on **strings, arrays, and objects**



# Expand string into array of characters
```javascript
a = [...'abdefg'] // [ 'a', 'b', 'd', 'e', 'f', 'g' ]
```

# Concatenate arrays
```javascript
const numbersOne = [1, 2, 3];
const numbersTwo = [4, 5, 6];
const numbersCombined = [...numbersOne, ...numbersTwo];
```

# Store part of an array in variables
* Assign the first and second items from numbers to variables and put the rest in an array:
```javascript
const numbers = [1, 2, 3, 4, 5, 6];
const [one, two, ...rest] = numbers;
```

# Works on objects
```javascript
const myVehicle = {
  brand: 'Ford',
  model: 'Mustang',
  color: 'red'
}

const updateMyVehicle = {
  type: 'car',
  year: 2021, 
  color: 'yellow'
}

const myUpdatedVehicle = {...myVehicle, ...updateMyVehicle}
```


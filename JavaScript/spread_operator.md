
# Spread operator
* `...` is the spread operator
* Used to unpack the elements of an array or object:
    * `[e1, e2, e3] => e1, e2, e3` 
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


# Destructing assignment
* The destructuring assignment syntax is a JavaScript expression that makes it
  possible to unpack values from arrays, or properties from objects, into
  distinct variables.

**All examples**
```javascript
const [a, b] = array;
const [a, , b] = array;
const [a = aDefault, b] = array;
const [a, b, ...rest] = array;
const [a, , b, ...rest] = array;
const [a, b, ...{ pop, push }] = array;
const [a, b, ...[c, d]] = array;

const { a, b } = obj;
const { a: a1, b: b1 } = obj;
const { a: a1 = aDefault, b = bDefault } = obj;
const { a, b, ...rest } = obj;
const { a: a1, b: b1, ...rest } = obj;
const { [key]: a } = obj;

let a, b, a1, b1, c, d, rest, pop, push;
[a, b] = array;
[a, , b] = array;
[a = aDefault, b] = array;
[a, b, ...rest] = array;
[a, , b, ...rest] = array;
[a, b, ...{ pop, push }] = array;
[a, b, ...[c, d]] = array;

({ a, b } = obj); // parentheses are required
({ a: a1, b: b1 } = obj);
({ a: a1 = aDefault, b = bDefault } = obj);
({ a, b, ...rest } = obj);
({ a: a1, b: b1, ...rest } = obj);

```

## const { a, b } = obj;
* a and b must be properties of obj


# Useful 
* break - breaks out of a loop or switch statement
* continue - breaks one iteration (in the loop), if a specified condition occurs, and continues with the next iteration in the loop

# Types of loops
* for - loops through a block of code a number of times
* for/in - loops through the properties of an object
* for/of - loops through the values of an iterable object
* while - loops through a block of code while a specified condition is true
* do/while - also loops through a block of code while a specified condition is true
* forEach - loops through the values of an iterable object. It lets you loop over array contents
* map - loops through the values of an iterable object. It lets you loop over array contents and modify the array


# Loop scope
```javascript
var i = 5;

for (var i = 0; i < 10; i++) {
  // i start = 0
}

// Here i is 10
```


# For in loop
* Used to loop through the **properties of an object**
* **NOTE:** Use standard for loop for looping through array indexes. 

## Interate trhough object keys
* Loops through the keys of an **object**
```javascript
for (let key in object) { }
```

## Iterate through array indexes
```javascript
for (let e in array ) { } // 1, 2, 3, 4, 5
```

# For of loop
* Used to iterate through the values of an **iterable object**
* All types is iterable except `null` and `undefined` 

## Interate through string
```javascript
for (let e of 'string') { } // s, t, r, i, n, g
```

## Iterate through array values
```javascript
array = [1, 2, 3, 4, 5]
for (let e of array ) { } // 1, 2, 3, 4, 5
```

# For each loop
* Can also use map 


**Note that the function takes 3 arguments:**
* The item value
* The item index (optional)
* The array itself (optional)

```javascript
const numbers = [45, 4, 9, 16, 25];
numbers.forEach(myFunction);
function myFunction(value, index, array) { }
```

#  While loop
```javascript
while (condition) {
  // code block to be executed
}
```

## Do while loop
* Cheks the statment after the loop

```javascript
let i = 0
do {
    i++
    console.log(i) // 1, 2, 3, 4, 5
} while (i < 5)
```
**Includes 5**



# Cool - Labeling loops
* Can target a specific loop with label. 
* XXX: should wrap in function and use return instead of break

```javascript
outerloop: for (let i = 0; i < 3; i++) {
  for (let j = 0; j < 3; j++) {
    console.log(i, j);
    if (i === 1 && j === 1) {
      break outerloop; // This breaks out of the outer loop
    }
  }
}
```




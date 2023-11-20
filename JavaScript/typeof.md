
**PS! Only usful for primitive data types**


# Typeof
* `typeof variable` - is an **operator**.   

## OBS!!
```javascript
typeof "John"                 // Returns "string"
typeof 3.14                   // Returns "number"
typeof NaN                    // Returns "number"
typeof false                  // Returns "boolean"
typeof [1,2,3,4]              // Returns "object"
typeof {name:'John', age:34}  // Returns "object"
typeof new Date()             // Returns "object"
typeof function () {}         // Returns "function"
typeof myCar                  // Returns "undefined" *
typeof null                   // Returns "object"
```


The data type of NaN is number
The data type of an array is object
The data type of a date is object
The data type of null is object
The data type of an undefined variable is undefined *
The data type of a variable that has not been assigned a value is also undefined *

**You cannot use typeof to determine if a JavaScript object is an array (or a date).**



# Primitive Data vs Complex Data

## Primitive data 
A primitive data value is a single simple data value with no additional
properties and methods.

The typeof operator can return one of these primitive types:

string
number
boolean
undefined


## complex data
**Can not use typeof to determine if a JavaScript object is an array (or a date).**

The typeof operator can return one of two complex types:

function
object
The typeof operator returns "object" for objects, arrays, and null.

The typeof operator does not return "object" for functions.

```javascript
typeof {name:'John', age:34} // Returns "object"
typeof [1,2,3,4]             // Returns "object" (not "array", see note below)
typeof null                  // Returns "object"
typeof function myFunc(){}   // Returns "function"

```

# The Data Type of typeof
The typeofoperator is not a variable. It is an operator. Operators ( + - * / ) do not have any data type.

But, the typeof operator always returns a string (containing the type of the operand).

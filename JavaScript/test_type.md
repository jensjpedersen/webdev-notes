


# Get the type of the variable 
```javascript

const typeOf = (obj) => Object.prototype.toString.call(obj).slice(8, -1).toLowerCase()

typeOf('')     // string
typeOf(0)      // number
typeOf()       // undefined
typeOf(null)   // null
typeOf({})     // object
typeOf([])     // array
typeOf(0)      // number
typeOf(() => {})  // function
```

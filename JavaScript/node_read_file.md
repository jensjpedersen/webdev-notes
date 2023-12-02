
# readFileSync()
when the fs.readFileSync() method is called the original node program stops
executing, and the node waits for the fs.readFileSync() function to get
executed, after getting the result of the method the remaining node program is
executed.

**Syntax**
```js
let text = fs.readFileSync(path, options)
```




# readFile()
* This method is asynchronous and returns the contents of the file in a callback.

```javascript
const fs = require('fs');

fs.readFile('./input.txt', (err, data) => {
    if (err) throw err; 
    console.log(data.toString())
})
```


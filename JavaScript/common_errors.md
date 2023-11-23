


# End stament with semicolon

**Wrong:**
```javascript
console.log('1')
(() => console.log('2'))()
```

* Nedd to terminate line with semicolon 
* Else it will be interpreted as `console.log('1')(() => console.log('2'))()`


**Correct:**
```javascript
console.log('1'); 
(() => console.log('2'))(); 
```



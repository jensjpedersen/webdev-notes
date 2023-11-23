
# SetTimeout
* `setTimeout` - is a built-in function that calls a function after a certain period of time

## Be careful of execution order!!!

```javascript
console.log('line 1'); 
setTimeout( () => console.log('line 2'), 0); 
console.log('line 3'); 
```

* The specified function will be placed in the event queue and executed after the current call stack is empty.

Output:
```
line 1
line 3
line 2
```


# Local storage
* browser - go to storage tab in firefox dev tools
* Can only store strings - can not store objects or arrays in local storage. 
* Should store as JSON string


* acess local storage from javascript
```javascript
console.log(localStorage);
```

# Avoid local storage conflicts
* avoid conflicts with other applications that use local storage

Use a unique key for your application: 
```javascript
const localStorageKey = 'applicationName';
```


# Methods
## Read from local storage
* If local storage is empty => returns null
* Can only read one key at a time
```javascript
console.log(localStorage.getItem('myKey'));
```

### Handle empty (null) storage
```javascript
let todyArray = JSON.parse(localStorage.getItem('todos')) || [];
```


## Write to local storage
* Write to local storage: 
```javascript
localStorage.setItem('myKey', 'myValue');
```

* Remove item from local storage: 
```javascript
console.log(localStorage.removeItem('myKey'));
```

* Clear all items from local storage: 
```javascript
console.log(localStorage.clear());
```

## Other local storage methods

* Check number of items in local storage: 
```javascript
console.log(localStorage.length);
```


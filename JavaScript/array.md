
# Splice

## Syntax
array.splice(index, howmany, item1, ....., itemX)

### Add elements

* At position 2, add 2 elements:

```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.splice(2, 0, "Lemon", "Kiwi");
```



### Remove elements

* At position 2, remove 2 items:

```javascript

const fruits = ["Banana", "Orange", "Apple", "Mango", "Kiwi"];
fruits.splice(2, 2);
```



# Check for empty objects
```bash
const isEmpty = obj => Reflect.ownKeys(obj).length === 0 && obj.constructor === Object

isEmpty({}) // true
isEmpty({ name: 'fatfish' }) // false
```

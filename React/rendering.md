

#  Updating count
* Count value is not rendered on the screen
* Only console is update
**This is why we need to use state**
State change will: 
* re-render the component
* update dom

```javascript
let count = 0

return (
    <button onClick={() => {
    count++; 
    console.log(count);
    }}> Incremnet: {count} </button>
)
```


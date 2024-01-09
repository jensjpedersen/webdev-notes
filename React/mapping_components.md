

# Key prop
* apped elements expect you to add a property called key to the element being
  repeated. 


```


# Wrong
Just passing index: 
* Works but not recommended
* 
 ```javascript
 
 return (
        <ul>
            {listItems.map((item, index)) => <li key={index}>{item}</li>}
        </ul>
    );
 ```
 

# Why key prop in react? 
* improve performance

# How to set key prop?
* Should be a unique id; not index. 
* Should be stable; not random.
* react uses key to identify which items have changed, are added, or are removed, in virtual dom. 



```javascript
...
{turtles.map((turtle, index) =>
<div key={turtle.name + "-" + index}>
...


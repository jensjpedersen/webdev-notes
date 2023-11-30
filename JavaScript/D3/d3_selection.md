
# D3 selection 
* is a library that allows you to select elements from the DOM and apply data to them.



# Select
* Metod chaning is a common pattern in D3 where you apply one or more methods to an element one after the other.


* select body 
```javascript
d3.select('body')
```


* method chaining
```javascript
d3.select('body').append('p').text('New paragraph!')
```


## Method chaining
* **With method chaining**
```javascript
const svg = selection.append('svg')
    .attr('width', 600)
    .attr('height', 600)
```

* Without method chaining
```javascript
const svg = selection.append('svg')
svg.attr('width', 600)
svg.attr('height', 600)
```





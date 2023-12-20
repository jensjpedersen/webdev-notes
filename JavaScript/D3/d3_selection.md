
# D3 selection 
* is a library that allows you to select elements from the DOM and apply data to them.



# Select
* The select method allows you to select an element from the DOM and apply data to it.
* Metod chaning is a common pattern in D3 where you apply one or more methods
  to an element one after the other.


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



# selectAll
* How to target spesific scope?:  
    * Use the svg group - `g`  
    * Can also target id or class

```javascript
body.selectAll('p') // Will select all p elements in the body
```

* The selectAll method allows you to select multiple elements from the DOM and
  apply data to them.


## Target spesific class
```javascript
d3.selectAll('.class1')
```



# Modifying selections
Modifying elements
Once you've made a selection you can modify the elements in it using the following functions:

| Name      | Behaviour                    | Example                                                                      |
|-----------|------------------------------|------------------------------------------------------------------------------|
| .style    | Update the style             | js d3.selectAll('circle').style('fill', 'red')                             |
| .attr     | Update an attribute          | js d3.selectAll('rect').attr('width', 10)                                  |
| .classed  | Add/remove a class attribute | js d3.select('.item').classed('selected', true)                            |
| .property | Update an element's property | js d3.selectAll('.checkbox').property('checked', false)                    |
| .text     | Update the text content      | js d3.select('div.title').text('My new book')                              |
| .html     | Change the html content      | js d3.select('.legend').html('<div class="block"></div><div>0 - 10</div>') |


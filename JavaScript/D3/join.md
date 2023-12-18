


# Adding Data with Join 

* .data - takes an array of data and joins it to the selection. Produces a data
  join. 
* .join -   

**Typically four methods are used in a data join:**
* .select defines the element that'll act as a container (or parent) to the joined HTML/SVG elements
* .selectAll - defines the type of element that'll be joined to each array
  element. This is initially empty, but will be created. 
* .data - defines the array that's being joined
* .join performs the join. This is where HTML or SVG elements are added and removed: 
* parameter`d` - from datum - Means: One entry in the data array

```javascript
const svg = d3.select("body")
    .append("svg")
    .attr("width", "100vw")
    .attr("height", "100vh");

let myData = [1, 2, 3, 4, 5];

d3.select('svg')
  .selectAll('circle')
  .data(myData)
  .join('circle')
  .attr('cx', (d) => d * 100)
  .attr('cy', 50)
  .attr('r', 5)
  .style('fill', 'orange');
```


## Example - Adding rectanges from array of objects

```javascript
const svg = d3.select("body")
    .append("svg")
    .attr("width", "100vw")
    .attr("height", "100vh");


const rect_array = []; 
for (let i = 0; i < 10; i++) {
    rect_array.push({
        x: i * 20,
        y: 0,
        width: 5,
        height: '100vh'
    });
}

svg.selectAll("rect").data(rect_array)
    .join("rect")
    .attr("width", d => d.width)
    .attr("height", d => d.height)
    .attr("x", d => d.x)
    .attr("y", d => d.y)
    .attr("fill", "red")

```



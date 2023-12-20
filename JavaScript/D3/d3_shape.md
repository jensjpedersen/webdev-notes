
# Symbols
XXX: add img




# D3 symbol
* Is centered at the origin (0,0) - use transform to move it
* Only works with **path elements**

## Example
```javascript
const svg = d3
    .select("body")
    .append("svg")
    .attr("style", "background-color: #eee")

svg
    .append("path")
    .attr("d", d3.symbol(d3.symbolCross))
    .attr("transform", "translate(50,50)")
```


## Types of symbols
[Symbols | D3 by Observable](https://d3js.org/d3-shape/symbol)

* symbolAsterisk
* symbolCircle
* symbolCross
* symbolDiamond
* symbolDiamond2
* symbolPlus
* symbolSquare
* symbolSquare2
* symbolStar
* symbolTriangle
* symbolTriangle2
* symbolWye

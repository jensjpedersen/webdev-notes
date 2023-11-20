
# SVG 
* scalable vector graphics

## Pros
* Vector graphics does not lose quality when scaled up or down. 
* Vector graphics are made up of paths, rather than individual pixels.
* Therefore: very good for data visualization.
* Easy to manipulate programmatically. 




# Creating svg
* z-index does not exist in svg. Figures are drawn in the order they are
  written in the code.

**HTML basics**
tag - text in the source code
element - created at runtime


## Circle 
```html
<svg>
<circle cs="50" cy="50" r="50" fill="red"></circle>
</svg>
```

cx - center x
cy - center y
r - radius
stroke - border color
stroke-width - border width

fill - fill color svg element

## Rectange

## Line
x1, y1, x2, y2
* need to set `stroke` to see the line

## Path 
[SVG Path](https://www.w3schools.com/graphics/svg_path.asp)

* Can be used to construct sequences of lines, arcs, etc.
* Used for graphing
* d attribute - used to define the path 

* The <path> element is used to define a path.

The following commands are available for path data:

* M = moveto
* L = lineto
* H = horizontal lineto
* V = vertical lineto
* C = curveto
* S = smooth curveto
* Q = quadratic Bézier curve
* T = smooth quadratic Bézier curveto
* A = elliptical Arc
* Z = closepath

**Upper case** - absolute position
**Lower case** - relative position (m, l, h, v, c, s, q, t, a, z)

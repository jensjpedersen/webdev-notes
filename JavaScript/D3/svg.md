
# SVG
* **All SVG attributes can be set as CSS properties.**


# Create svg with js 
```javascript
const svg_type = document.createElementNS('http://www.w3.org/2000/svg', 'svg_type');
```


# Svg elements
[SVG element reference - SVG: Scalable Vector Graphics | MDN](https://developer.mozilla.org/en-US/docs/Web/SVG/Element)
* rect
* circle
* mask 


## Circle
```xml
<circle cx="50" cy="50" r="40" stroke="black" stroke-width="3" fill="red" />
```

## Rect
```xml
<rect x="10" y="10" width="80" height="80" />
```

## Mask
[<mask> - SVG: Scalable Vector Graphics | MDN](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/mask)
* The <mask> element defines an alpha mask for compositing the current object into the background.
```xml
<mask id="mask">
  <rect x="0" y="0" width="100%" height="100%" fill="white" />
  <circle cx="50" cy="50" r="40" fill="black" />
</mask>
```



# SVG attributes

* `width and height` : Specifies the width and height of the SVG viewport.
* `fill` : Sets the fill color of a shape.
* `stroke and stroke-width` : Determines the stroke color and width of a shape.
* `opacity` 
* `transform` : Applies transformations such as translation, rotation, and scaling.
* `x and y`  : Defines the x and y coordinates of the SVG viewport origin.
```xml
<rect x="10" y="10" width="80" height="80" transform="rotate(45)" />
```
* `id`  
* `class` 
* `xmlns` : Defines the XML namespace.
```xml
<svg xmlns="http://www.w3.org/2000/svg">
  <!-- SVG content -->
</svg>
```




